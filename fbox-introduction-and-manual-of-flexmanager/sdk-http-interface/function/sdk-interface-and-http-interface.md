# SDK Interface and HTTP Interface



* \*\*\*\*[**Function Instruction**](https://docs.flexem.net/fbox/zh-cn/function/Images/SDKHttp.png) 

![](../../../.gitbook/assets/image%20%2864%29.png)

With the FServer solution, users can use the SDK interface or HTTP interface to obtain FBox data from the FlexCloud server or private cloud server to develop their own PC monitoring system or mobile APP.

 **Flexem SDK interface and HTTP interface have the following functions:**

* Use the function of real-time data push to read and write real-time data, alarm registration and historical data storage. 
* With real-time data push function, when the data changes, it is directly pushed to the computer client without polling and reading. 
* You can also use the historical data storage function to view and export historical data. 
* The FBox is verified by ID and password, which is used to distinguish and mark different FBoxes at different sites. 
* The SDK interface can also use the location information of the base station for positioning, and the user can resolve the location information by himself.

**The Difference between SDK Interface and HTTP Interface**

* The SDK interface is developed in the .net environment, and the scope of HTTP usage is wider; 
* HTTP can be used for PC-side and mobile APP development, while SDK is limited to computer-side development.
* SDK can use the base station information of 2G or 4G signal to locate, HTTP does not have this function. 
* Neither interface has remote download and remote configuration functions. If you need this function, please use FBox PC Client software.
* For the requirements of programmers, the SDK method needs to be familiar with the development of the .net platform, while the HTTP method requires developers to be familiar with the simple HTTP protocol.
* Our message push mechanism uses the SignalR framework, so you need to know about it regardless of the SDK or HTTP method.

