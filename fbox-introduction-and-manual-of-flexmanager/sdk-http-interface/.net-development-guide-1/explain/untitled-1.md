# Initialization

Log in to the server through configuration parameters

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
        public static string ClientId { get; set; } = "ClientId";
        public static string ClientSecret { get; set; } = "ClientSecret";
        public static string UserName { get; set; } = "UserName";
        public static string Password { get; set; } = "Password";
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
            //Create object and initialize
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
        }
    }
    class Program
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                //The start method is called, the signalr connection object is established internally, and Restart only needs to be executed globally once.
                fbox.Start();

                Console.ReadLine();
            }
        }
    }
}
```

When creating an IFBoxClientManager instance and initializing it, you need to provide the following parameters:`clientId`,`clientsecret`,`username`,`password`,`Id server`,`App server`, and`Hdata Server`  
`username`,`password`are the username and password of FlexManager  
`clientId`,`clientsecret`are the account and password for finding sales application  
`Id server`,`App server`, and`Hdata Server`will remain unchanged if they are public cloud, but private cloud will be changed to the corresponding address

