# Code Demo

 [C\# SDK Demo下载](http://download.flexem.net/fbox/sdk/csharp/demo.7z)  


 [Java SDK Demo下载](http://download.flexem.net/fbox/sdk/java/Java-Demo.7z)  


 1、java demo使用请先阅读文件下的README文件。  
 2、C\#的依赖包FBoxClientDriver与FBoxClientDriver.Contract在demo文件中的Nuget文件夹下，引用本地依赖包即可  
 3、Signalr要保持长连接，用单例开发  


 **C\# SDK使用说明**  


 特别说明：  
 1、仅供合作伙伴交流使用。  
 2、此 C\# SDK 适用于 Visual Studio版本号15.3及以上。  
 3、此 C\# SDK 中为Console程序（.NET Core）。  
 4、接口返回401均为token过期。需要根据refresh\_token调重新登录接口刷新access\_token后重试。refresh\_token有效期为30天。java demo和C\# SDK已处理刷新token流程和signalr重连问题  


 **第一步：引入NuGet依赖包**

`FBoxClientDriver`

`FBoxClientDriver.Contract`  


**例如引入FBoxClientDriver包**  


* **方式一**

   在Visual Studio2017命令行中执行如下语句  


   `PM> Install-Package FBoxClientDriver`  

* **方式二**  


   在Visual Studio2017中导入项目，在NuGet包库中引入依赖包名，如下图。

 **第二步：引入项目文件**  


* 在Visual Studio的界面中，右键单击您的解决方案。
* 单击添加 -&gt; 现有项目。
* 在弹出的对话框中，选择C\# SDK中项目文件（`FBoxDemo.cs`与`Program.cs`），单击打开。

## **代码示例** <a id="&#x4EE3;&#x7801;&#x793A;&#x4F8B;"></a>

以下代码示例展示了调用C\# SDK的几个主要步骤：

* 创建全局变量
* 创建IFBoxClientManager、ILogger实例并初始化。
* 开启指定盒子所有监控点数据推送
* 侦听盒子状态变更事件
* 侦听实时数据变更事件
* 发起请求并处理返回。
* 释放资源

```text
using System;
using System.Collections.Generic;
using System.Threading.Tasks;
using FBoxClientDriver;
using FBoxClientDriver.Contract;
using FBoxClientDriver.Impl;
using Microsoft.Extensions.Logging;

namespace SDKDEMO
{
    //创建配置参数
    public class FBoxClientParameters
    {
        public static string ClientId { get; set; } = "";       //找销售申请
        public static string ClientSecret { get; set; } = "";   //找销售申请
        public static string UserName { get; set; } = "";       //FlexManager注册
        public static string Password { get; set; } = "";       //FlexManager注册
        //服务器地址，公有云不变，私有云改为对应服务器地址
        public static string IdServer { get; set; } = "https://account.flexem.com/core";
        public static string MainServer { get; set; } = "http://fbox360.com";
        public static string HdataServer { get; set; } = "http://fbhs1.fbox360.com";
    }

    public class FBoxDemo : IDisposable
    {
        private readonly IFBoxClientManager _fbox;
        private readonly ILogger _logger;
        private readonly string boxNo = "300015050009"; //以这个盒子为例

        public FBoxDemo(ILoggerFactory loggerFactory)
        {
            //创建ICredentialProvider、FBoxClientManager对象并初始化
            _logger = loggerFactory.CreateLogger();

            ICredentialProvider provider =
                new DefaultCredentialProvider(FBoxClientParameters.ClientId,FBoxClientParameters.ClientSecret,FBoxClientParameters.UserName,FBoxClientParameters.Password);
            _fbox = new FBoxClientManager(FBoxClientParameters.IdServer,FBoxClientParameters.MainServer,FBoxClientParameters.HdataServer,provider,Guid.NewGuid().ToString("N"), loggerFactory);
            //侦听FBox状态变更事件
            _fbox.BoxConnectStateChanged += _fbox_BoxConnectStateChanged;
            //侦听实时数据变更事件
            _fbox.DataMonitorValueChanged += _fbox_DataMonitorValueChanged;
        }

        private void _fbox_DataMonitorValueChanged(object sender, IList e)
        {
            foreach (var dmon in e)
                Console.WriteLine($"dmv:{dmon.Uid}:{dmon.Value},{dmon.Status}");
        }

        private void _fbox_BoxConnectStateChanged(object sender, IList e)
        {
            //NewState：1、2是盒子在线状态。0、3为盒子不在线状态，根据盒子状态对盒子进行开点操作
            foreach (var stateItem in e)
            {
                Console.WriteLine($"{stateItem.BoxNo},{stateItem.NewState}");
            }
        }

        public async Task Go()
        {
            try
            {
                //初始化SDK，内部建立signalr连接对象，Restart只需全局执行一次。
                await _fbox.Restart();

                //盒子掉线后，等盒子重新上线后均需要重新开点
                await _fbox.StartAllDataMonitorPointsOnBox(new BoxArgs(boxNo));  //开启FBox所有监控点数据推送

                //逻辑代码
                //例如： 
                //var groups = await _fbox.GetDataMonitorGroups(new GetDMonitorGroupsArgs()
                //{
                //  BoxNo = boxNo                                   //盒子号
                //});
                //foreach (var group in groups)
                //{
                //  Console.WriteLine(group.DataMonitorDefinitions); //监控点组下的监控点条目Id
                //  Console.WriteLine(group.Uid);                    //监控点组的Id
                //  Console.WriteLine(group.GroupName);              //监控点组的名称
                //}
            }
            catch (Exception e)
            {
                Console.WriteLine(e);
                throw;
            }
        }

        public void Dispose()
        {
            _fbox.BoxConnectStateChanged -= _fbox_BoxConnectStateChanged;
            _fbox.DataMonitorValueChanged -= _fbox_DataMonitorValueChanged;
            _fbox?.Dispose();
        }
    }
}
```

在创建IFBoxClientManager实例并初始化时，您需要提供一下参数：`ClientId`、`ClientSecret`、`Username`、`Password`、`IdServer`、`MainServer`、和`HdataServer`  
`Username`、`Password`为FBox客户端的账号、密码  
`ClientId`、`ClientSecret`为找销售申请的开发者账号、密码  
`IdServer`、`MainServer`、和`HdataServer`若公有云的话不变，私有云改为对应地址

