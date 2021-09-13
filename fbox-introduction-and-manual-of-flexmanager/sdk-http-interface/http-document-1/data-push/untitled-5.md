# Data Push Related（SignalR）

* **Function Description**

  The real-time data of all monitoring points are actively pushed by the server, and the client can control to open one or several monitoring groups. After opening, when the data in the opened group changes \(the change of the dead zone setting needs to exceed the dead zone range\) The server actively pushes to the client. The push function needs to rely on the signalR library.

* **.NET** Official website document**：**

   `https://www.asp.net/signalr`

> **.NET class library, please use the Nuget tool in Visual Studio to download Microsoft.AspNet.WebApi.Client.**

* **JAVA Sample**

   `https://github.com/flexem/FBox-SDKSamples/tree/master/Java`

**Create signalR Link**

* **Request Address**

  **URL：**`signalRUrl obtained from FBox Lists`see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details

   **querystring:** `at={token}&cid={X-FBox-ClientId}`  


  | Filed Name | Type | Description |
  | :--- | :--- | :--- |
  | token | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

   **SignalR service's Hub name ：clientHub**  

**NOTE**  
 1. The token validity period is two hours. 401 means the token expired. You need to log in to the interface again according to the refresh\_token adjustment, refresh the access\_token, and then reconnect to SignalR. The refresh\_token is valid for 30 days.。  
 2. The java demo and C\# SDK have dealt with the issue of token refresh and Signalr reconnection. If you don't use the demo, you need to handle this process yourself in the program.  
 3.Signalr should maintain a long connection and use singleton development

