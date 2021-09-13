# Code Sample

 [C\# SDK Demo ](http://download.flexem.net/fbox/sdk/csharp/demo.7z)Download

 [Java SDK Demo](http://download.flexem.net/fbox/sdk/java/Java-Demo.7z) Download

1. To use java demo, please read the README file under the file first.  
 2. C\# dependency packages FBoxClientDriver and FBoxClientDriver.Contract are in the Nuget folder in the demo file, and you can reference the local dependency package  
 3. Signalr should maintain a long connection and use singleton development

 **C\# SDK Using Instruction**

 **Special Description**：  
 1. Only for partner communication.  
 2. This C\# SDK is suitable for Visual Studio version 15.3 and above.  
 3. This C\# SDK is the Console program \(.NET Core\).  
 4. If the interface returns 401, the token is expired. You need to log in to the interface again according to the refresh\_token adjustment, refresh the access\_token and try again. The refresh\_token is valid for 30 days. The java demo and C\# SDK have dealt with the token refresh process and signalr reconnection issues

 **Step 1：import NuGet dependency package**

`FBoxClientDriver`

`FBoxClientDriver.Contract`  


**For example import FBoxClientDriver package**

* **Method 1**

   Execute the following statement in the Visual Studio2017 command line  


   `PM> Install-Package FBoxClientDriver`  

* **Method 2**

   Import the project in Visual Studio 2017, and import the dependent package name in the NuGet package library, as shown in the figure below.

![](../../../../.gitbook/assets/image%20%2818%29.png)

 **Step 2：Import project files** 

* In the Visual Studio interface, right-click on your solution.
* Click Add -&gt; Existing Project.
* In the pop-up dialog box, select the project files \(`FBoxDemo.cs and Program.cs),` and click Open.

## **Code Sample** <a id="&#x4EE3;&#x7801;&#x793A;&#x4F8B;"></a>

The following code example shows the main steps of invoking the C\# SDK:

* Create global variables
* Create and initialize IFBoxClientManager and ILogger instances.
* Turn on data push of all monitoring points in the specified box
* Listen to box state change events
* Listen to real-time data change events
* Initiate the request and process the return.
* Release resources

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
    //Create configuration parameter
    public class FBoxClientParameters
    {
        public static string ClientId { get; set; } = "";       //Find a sales application
        public static string ClientSecret { get; set; } = "";   //Find a sales application
        public static string UserName { get; set; } = "";       //FlexManager register
        public static string Password { get; set; } = "";       //FlexManager register
        //Server address, the public cloud remains unchanged, the private cloud is changed to the corresponding server address
        public static string IdServer { get; set; } = "https://account.flexem.com/core";
        public static string MainServer { get; set; } = "http://fbox360.com";
        public static string HdataServer { get; set; } = "http://fbhs1.fbox360.com";
    }

    public class FBoxDemo : IDisposable
    {
        private readonly IFBoxClientManager _fbox;
        private readonly ILogger _logger;
        private readonly string boxNo = "300015050009"; //Take this box as an example

        public FBoxDemo(ILoggerFactory loggerFactory)
        {
            //Create ICredentialProvider、FBoxClientManagerObject and initialize
            _logger = loggerFactory.CreateLogger();

            ICredentialProvider provider =
                new DefaultCredentialProvider(FBoxClientParameters.ClientId,FBoxClientParameters.ClientSecret,FBoxClientParameters.UserName,FBoxClientParameters.Password);
            _fbox = new FBoxClientManager(FBoxClientParameters.IdServer,FBoxClientParameters.MainServer,FBoxClientParameters.HdataServer,provider,Guid.NewGuid().ToString("N"), loggerFactory);
            //Listen to FBox status change events
            _fbox.BoxConnectStateChanged += _fbox_BoxConnectStateChanged;
            //Listen to real-time data change events
            _fbox.DataMonitorValueChanged += _fbox_DataMonitorValueChanged;
        }

        private void _fbox_DataMonitorValueChanged(object sender, IList e)
        {
            foreach (var dmon in e)
                Console.WriteLine($"dmv:{dmon.Uid}:{dmon.Value},{dmon.Status}");
        }

        private void _fbox_BoxConnectStateChanged(object sender, IList e)
        {
            //NewState：1, 2 is the online status of the box. 0, 3 means the box is not online, open the box according to the box status
            foreach (var stateItem in e)
            {
                Console.WriteLine($"{stateItem.BoxNo},{stateItem.NewState}");
            }
        }

        public async Task Go()
        {
            try
            {
                //The SDK is initialized, the signalr connection object is established internally, and Restart only needs to be executed globally once.
                await _fbox.Restart();

                //After the box is disconnected, it needs to be opened again after the box is online again
                await _fbox.StartAllDataMonitorPointsOnBox(new BoxArgs(boxNo));  //开Enable data push of all monitoring points of FBox

                //Logic Code
                //For example: 
                //var groups = await _fbox.GetDataMonitorGroups(new GetDMonitorGroupsArgs()
                //{
                //  BoxNo = boxNo                                   //Box number
                //});
                //foreach (var group in groups)
                //{
                //  Console.WriteLine(group.DataMonitorDefinitions); //Monitoring point entry Id under the monitoring point group
                //  Console.WriteLine(group.Uid);                    //Id of the monitoring point group
                //  Console.WriteLine(group.GroupName);              //The name of the monitoring point group
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

When creating an IFBoxClientManager instance and initializing it, you need to provide the following parameters:`ClientId`,`ClientSecret`,`Username`,`Password`,`IdServer`,`MainServer`, and`HdataServer`  
`Username`,`Password`are the username and password of FBox client  
`ClientId`,`ClientSecret`are the account and password of the developer applied from sales.  
`IdServer`,`MainServer`, and`HdataServer`If the public cloud is unchanged, the private cloud will be changed to the corresponding address

