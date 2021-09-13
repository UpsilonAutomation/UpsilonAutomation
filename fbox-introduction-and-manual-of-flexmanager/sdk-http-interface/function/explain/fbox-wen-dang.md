# Sample Code

## Special Description <a id="&#x7279;&#x522B;&#x8BF4;&#x660E;"></a>

1. Applicable to Visual Studio version number
2. Need to import [NuGet](https://docs.microsoft.com/zh-cn/nuget/) dependency package`FBoxClientDriver`,`FBoxClientDriver.Contract`

The steps in the sample code are as follows:

* Configuration parameter
* Create DefaultCredentialProvider object
* Create FBoxClientManager object
* Log in to the server
* Listen to box state change events
* Listen to real-time data push change events
* Open all monitoring points of the box data push
* Definition method
* Call method

## **Sample Code as below：** <a id="&#x793A;&#x4F8B;&#x4EE3;&#x7801;&#x5982;&#x4E0B;"></a>

**NOTE:**  
Need to open point before data push

```text
using System;
using System.Collections.Generic;
using System.Linq;
using System.Threading;
using FBoxClientDriver;
using FBoxClientDriver.Contract;
using FBoxClientDriver.Impl;

namespace SDKDEMO
{
    //Configure parameter
    public class FBoxClientParameters
    {
        public static string ClientId { get; set; } = "";
        public static string ClientSecret { get; set; } = "";
        public static string UserName { get; set; } = "";
        public static string Password { get; set; } = "";
        public static string IdServer { get; set; } = "https://account.flexem.com/core";
        public static string MainServer { get; set; } = "http://fbox360.com";
        public static string HdataServer { get; set; } = "http://fbhs1.fbox360.com";
    }

    public class FBoxDemo : IDisposable
    {
        private readonly IFBoxClientManager _fbox;
        private readonly string boxNo = "300015050009"; // Take this as example 

        public FBoxDemo()
        {
            //Creat object and initialize
            var provider =
                new DefaultCredentialProvider(FBoxClientParameters.ClientId, FBoxClientParameters.ClientSecret,
                    FBoxClientParameters.UserName, FBoxClientParameters.Password);
            _fbox = new FBoxClientManager(FBoxClientParameters.IdServer, FBoxClientParameters.MainServer,
                FBoxClientParameters.HdataServer, provider, Guid.NewGuid().ToString("N"), null);
        }

        public void Dispose()
        {
            _fbox?.Dispose();
        }

       /// 
        /// Turn on 
        /// 
        public void Start()
        {
            //The SDK is initialized, the signalr connection object is established internally, and Restart only needs to be executed globally once.
            _fbox.Restart().Wait();
            //Listen to the box state change event
            _fbox.BoxConnectStateChanged += _fbox_BoxConnectStateChanged;
            //Listen to real-time data change events
            _fbox.DataMonitorValueChanged += _fbox_DataMonitorValueChanged;
        }

        /// 
        /// Real-time data change function
        /// 
        /// 
        /// 
        private void _fbox_DataMonitorValueChanged(object sender, IList e)
        {
            foreach (var dmon in e)
                Console.WriteLine($"dmv:{dmon.Uid}:{dmon.Value},{dmon.Status}");
        }

        /// 
        /// Box state change function
        /// 
        /// 
        /// 
        private void _fbox_BoxConnectStateChanged(object sender, IList e)
        {
            //NewState：1, 2 is the online state of the box. 0, 3 means the box is not online, open the box according to the box status
            foreach (var stateItem in e)
            {
                Console.WriteLine($"{stateItem.BoxNo},{stateItem.NewState}");
            }
        }

        /// 
        /// Turn on all the monitoring points of box
        /// 
        public void StartAllDMonData()
        {
            //Every time the box goes offline, it needs to be reopened after it goes online again
            try
            {
                _fbox.StartAllDataMonitorPointsOnBox(new BoxArgs(boxNo)).Wait();//boxNo is box number
            }
            catch (Exception ex)
            {
                switch (ex.Message)
                    {
                        // Not logged in to the server, please Restart() first
                        case "Box server not found.":; break;
                        // No box with BoxNo serial number found under the current account
                        case "Not Found":; break;
                        default:; break;
                    }
            }
        }

        /// 
        /// 获取盒子分组和盒子信息
        /// 
        public void GetBoxGroups()
        {
            var grpList = _fbox.GetBoxGroups().Result;
            foreach (var grp in grpList)
            {
                Console.WriteLine(grp.Uid);                 // the Uid of box group
                Console.WriteLine(grp.Name);                // the name of of box group
                foreach (var box in grp.Boxes)              // Traverse the set of boxes under the group
                {
                    Console.WriteLine(box.BoxId);           // Box Id
                    Console.WriteLine(box.Alias);           // Box name
                    Console.WriteLine(box.BoxNo);           // Box number
                    Console.WriteLine(box.ConnectionState); // When getting the box state, it cannot be used as a real-time state, and this interface cannot be called all the time as a box state change. Please use SignalR to push the box state change in real time
                    Console.WriteLine(box.NetworkType);     // Network Type 1: Network, 2: 2G, 3: 3G (this is not supported), 4: Wifi, 5: 4G
                    Console.WriteLine(box.Disabled);        // Whether the box is disabled
                    Console.WriteLine(box.ApiBaseUrl);      // ApiBaseUrl server address
                    Console.WriteLine(box.SignalrUrl);      // SignalR server address
                    Console.WriteLine(box.Owned);           // Is it the owner
                    Console.WriteLine(box.BoxType);         // Box tyepe， 0：standard box，1：mini box,2:Lite 3：VPN box
                }
            }
        }
        //Define method
    }
    class Program
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                fbox.Start();
                fbox.StartAllDMonData();
                fbox.GetBoxGroups();
                //Call the defined method
                Console.ReadLine();
            }
        }
    }
}
```

When creating an IFBoxClientManager instance and initializing it, you need to provide the following parameters:`clientId`,`clientsecret`、`username`,`password`,`Id server`,`App server`,和`Hdata Server`  
`username`,`password`are account and password for FlexManager  
`clientId`,`clientsecret`are the account and password applied from the sales.  
`Id server`,`App server`, and`Hdata Server`If the public cloud is unchanged, the private cloud will be changed to the corresponding address

