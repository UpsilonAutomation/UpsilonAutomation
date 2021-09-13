# Summary of Common Problems

## Login interface <a id="&#x767B;&#x5F55;&#x63A5;&#x53E3;"></a>

**🙋How to fill in the two parameters of client\_id and client\_secret?**

👉 Find a sales application account.

**🙋 Is there a limit on the calling frequency of the login interface？**

👉 The API can be called at multiple points at the same time. There are no restrictions on the interface. The interface is adjusted according to the server's resources and is not constant. Currently, there is no fixed frequency limit, and there is no problem with normal business calls.。

**🙋 There are tens of thousands of sub-users under a customer, and 1,000 users are requested to log in under the sub-users. In the client platform, there are actually 1,000 logins, but on a server, the login interface is called once, and 1,000 are actually logged in at the same time. Users, will this cause frequent interface calls?**

👉 In fact, we allow multiple logins. You can log in with the same token through our login. At the same time, less than 100 users are allowed to log in. The customer has to ensure the performance of the interface. We can let the operation and maintenance add IP whitelist, but there is no guarantee that more than 100 users will be temporarily blocked if there is a problem with the login.

**🙋 Use cookies to handle login and call other interfaces?**

👉Our server does not process authentication based on cookies, but includes Authorization in the http header of the request, and then we can call our interface. The access token is valid for 2 hours. After logging in to the platform for 5 minutes with multiple consecutive login errors, the account will be locked for 5 minutes. After changing the account or password, refresh\_Token immediately becomes invalid, and access\_Token needs to wait 2 hours to expire. The actual processing is based on the 401toekn invalidation returned by the interface.

**🙋 The postman test interface reports could not get any response error?**

👉 The Bearer and token of the Authorization parameter can only have one space and multiple spaces, resulting in an error.

## Write Value Process <a id="&#x5199;&#x503C;&#x6D41;&#x7A0B;"></a>

🙋**About the frequency of obtaining the monitoring point value?** 

👉 This interface can be used to obtain the monitoring point value, that is, to obtain the user's real-time data. This interface has a frequency limit. It is recommended not to exceed once a second. If it exceeds a certain frequency, Ng will block IP processing.

🙋 **How many monitoring points can be added to the interface at a time?**

👉 The current interface can add up to 20 monitoring points at a time. This is a limitation of the interface, but it can be added multiple times.

🙋 **How to remotely control all the device switches?**

👉 The monitoring point of the box and the device controller are related through the plc address. Controlling the monitoring point can control the switch of the device, which is to write a value \(change the value\) to the monitoring point.

🙋 **After calling the write interface, the device does not start?**

👉 Check whether the http status of the write value interface is 200 instead of 200. Check the parameter according to the status code returned by the interface. If it is 200, you need regional technical support to help find the reason \(maybe the monitoring point is configured incorrectly\).

🙋 **Why is it not recommended to call http to get monitoring point value interface?**

👉 Through the name or id of the monitoring point, you can query the data of the monitoring point and obtain the data of the monitoring point. Because this method will be called frequently, the server stability is relatively large, and when it has a certain impact on our server, the IP processing will be blocked , It is not recommended to use, it is recommended to use signalr to push.

🙋 **Call to get monitoring point value interface or other interface returns 429 \(access interface frequency is too fast\)?**

👉 The interface frequency will be adjusted according to the server resources, it is not constant, and there is currently no fixed frequency limit. Calls on normal business are fine. This is just the http status code. Use the log to save the interface parameters and status code. It is convenient to analyze later.

🙋 **Can I add monitoring points after the box is offline?**

👉 When the box is online, directly send the configuration to the box. If the box is not online, the server records it first, and then sends it after the box is online \(offline task\).

🙋 **How to control the interface to only obtain certain monitoring points?**

👉 The interface is currently not controlled. It can be controlled through the sharing function. First, share the monitoring points that need to be shared, set the permissions of the sharing engineer, and then add the monitoring points that do not need to be shared. After each sharing, the monitoring point id of the sharing account will be regenerated.

🙋 **The newly added monitoring point is successfully opened, but the new data point is not pushed?**

👉 Open the box before the mission is completed, you can only wait for a few seconds.

🙋 **Call the write value interface, the call interface does not respond?**

👉 When the write value interface is called, there is a box to complete the feedback. If the box has been unresponsive, the server http timeout will be about 1 minute

🙋 **Call the write value interface, modify the monitoring point, the value of other monitoring points also changed?**

👉 Calling the interface to write values ​​and changing the data of other monitoring points does not exist. The first step is to check whether the monitoring points of the platform are set correctly, and manually change the value on the platform. If the value of a monitoring point is manually changed on the platform, The values ​​of other monitoring points have also changed, indicating that the monitoring point is configured incorrectly. Check the data type and address of the monitoring point. If the data of other monitoring points has not changed, then there is a problem with the customer submitting the code, and the customer needs to do so. Check the code again.

🙋 **How to write a value to the device? Why does the value written to the monitoring point on FlexeManager change back?**

👉 The attribute of the monitoring point of the box already includes the switch of the device controller. Controlling the monitoring point can control the switch of the device. Some points cannot be written. If they change back, it means that they cannot be written. Mainly depends on the address type. Configure according to the situation. Need to find someone who specializes in automation programs to read the instructions.

🙋 **How does the box control the switch of the device?**

👉 There are many instructions for customer types. We can only tell the customer the data type of the monitoring point, and configure it according to the actual situation. The monitoring point needs to find the system integrator who is specifically responsible for the project or the programmer who specializes in automation. This kind of problem needs to be confirmed by this type of person.

🙋 **Add a new monitoring point, the interface return code is 400, and the X-FBox-Code under Headers is 9999, or 10050**

👉 9999: Body format is set \[{},{}\], multiple monitoring points can be added at once. 10050, the devAlias ​​parameter of the new monitoring point needs to be filled in the alias of the driver

🙋 **About X-FBox-ClientId**

👉 Check Appendix 1, Guid or UUID code generation in the program. The postman debugging interface can be generated by Baidu.

## Obtain Information Interface <a id="&#x83B7;&#x53D6;&#x4FE1;&#x606F;&#x63A5;&#x53E3;"></a>

🙋 **Why can't I get the address and location information of the box when calling the interface to get the address location of the box?**

👉 If the address obtained by the customer is automatically located on the platform, it can be queried in the interface. If the address is obtained manually by the customer on the platform, the information cannot be obtained in the interface. \(Call the interface to get the location of the box, use the cellular network box support, 2G or 4G module box \(need to plug in the phone card\) online will upload the geographic location, the server will save, so the offline box can also display the geographic location, only The geographic location will be updated when it goes online again. The Ethernet cannot obtain geographic information. The manual positioning information cannot be obtained through the interface, and the interface returns 424 \(only our records\). The latitude and longitude are Baidu map, Mars coordinate system\).

🙋 **Can the group of monitoring points have the same name? Will the information of configuring monitoring points be affected as well?**

👉 The group of monitoring points cannot have the same name. The configuration information of the same monitoring point is the same, and signalr will push multiple results.

## Remote Download <a id="&#x8FDC;&#x7A0B;&#x4E0B;&#x8F7D;"></a>

🙋 **Device management interface for remote download?**

👉 Download box driver interface, network plc set ip and port, com is other parameters. Whether it is a serial port or a network plc, the advanced field is passed null, and the optimal default configuration suitable for the box will be set here. It is not recommended that you modify the communication parameters. This is related to PLC communication. It is recommended to leave the default one. Using the interface to download plc will overwrite all previous drivers. You need to get the original driver first, splice \[{},{}\] and then send it back to the server. The box where the driver is configured for the first time sends the driver through the interface, and the device source needs to be set to the server.

🙋 **Download the PLC driver interface, the interface return code is 400, and the X-FBox-Code under Headers is 9999**

👉 The body format is a collection \[{},{}\], and every time it is sent, the previous driver will be overwritten.

🙋 **Call the download driver interface**

👉 Use the interface to download the plc driver, which will overwrite the plc driver originally issued. So it needs to be spliced first \[{},{}\]

## Alarm Interface <a id="&#x62A5;&#x8B66;&#x63A5;&#x53E3;"></a>

🙋 **How to get the number of alarm entries?**

👉 Get the total number of alarms, currently not available, you can count it yourself in the alarm list.

🙋 **Added alarm registration, how to notify the device alarm?**

👉 After adding an alarm entry, register an alarm contact in FlexManager to receive alarm notifications. Or the secondary development program listens to signalr's alarm trigger and recovery event reception.

🙋 **The box is offline, will the alarm data generated by the device be lost?**

👉 The child will store the alarm data locally, and after the box goes online, it will report to the server again, and the server will push the alarm data generated when it goes online. It will be pushed in different channels.

🙋 **What is the mechanism of alarm trigger push and alarm restoration?**

👉 The alarm information will only be reported once. If it is greater than a certain value for a long time, it will not be pushed. You need to wait for the data to recover.

🙋 **What is the reason for deleting the alarm group report 406?**

👉 1. The alarm points under the alarm group cannot be deleted.

```text
2. The names of the alarm points under the same box cannot be repeated.
```

🙋 **Will adding monitoring points or alarm points exceed the limit, will it have any impact?**

👉 The entry exceeds the limit. The box is due to too many collection queues, processing efficiency is low, and it may also cause the box to restart.

🙋 **Is there a limit on the number of alarm registrations added to the interface?**

👉 The length of the array should not exceed 20 . 🙋 The customer has deployed two servers and received two pieces of alarm data. How to distinguish whether they are the same data type?

👉 The alarm will only be reported once when the alarm is triggered. The alarm messages are all reported by the box. The condition data is exactly the same and needs to be filtered by you. It is better to judge by several fields, such as value.

🙋 **What if a customer wants to get real-time alarm records?**

👉 The alarm record is pushed through time, and the customer does not need to actively call the interface to obtain it. The historical record is only a record and cannot be regarded as an instant alarm.

🙋 **Call the alarm record data interface, there is a frequency limit, can we check and call the alarm record interface once an hour?**

👉 If real-time data push is connected, just add these two alarm event listeners. These two events have no preconditions, just listen. Once an hour is okay, but if the number of boxes is very large, you must control them and not call them concurrently. The main reason is that the alarm history record interface consumes server resources. Public cloud customers have a large amount of data, frequent calls, and insufficient public cloud server resources.

🙋 **What is alarm restoration?**

👉 Alarm restoration means that the current value does not meet the alarm conditions.

## Historical Record Interface <a id="&#x5386;&#x53F2;&#x8BB0;&#x5F55;&#x63A5;&#x53E3;"></a>

🙋 **How long can historical data be stored? Will the query speed slow down?**

👉 The historical data is stored on the server for 3 months. After the data is accumulated, querying the historical data will not slow down.

🙋 **Historical data can only be obtained for a maximum of 3 months. What is the method to obtain data from a longer time?**

👉 It is recommended that customers build their own servers and store the received real-time data as historical data.

🙋 **Can historical data be obtained by third-party methods? How to query the number of historical records?**

👉 To obtain historical data, you must first register historical entries, and then call the interface for obtaining historical data. Each historical entry can add 16 acquisition channels. Querying historical data is to query the channel data under the historical entry, with the most channels. 16 pieces.

🙋 **When obtaining historical data, the platform displays N/A, but the data received by the interface is empty?**

👉 The N/A displayed on the FlexManager platform is not given by the plc, so the data is empty on the interface.

🙋 **If the online box under the account is offline, will the historical data still be cached?**

👉 Historical data can be cached, but the offline cache of historical data is limited. The more historical entries, the shorter the collection interval and the shorter the offline storage time. The box storage space is limited. The maximum support for 50,000 data is to be After the box goes online, the data generated offline and the newly generated historical data are divided into two channels and reported to the server, which do not affect each other. Offline data is also slowly transferred in the background, one packet by packet. \*

🙋 **I have registered a history entry in the history record, why can’t I find it in the interface?**

👉 After adding a history record entry, the box will collect 100 locally or report the history record to the server in 20 minutes before calling the http interface for query.

🙋 **Get history data interface parameters?**

👉 begin and end are UTC in milliseconds, and limit is the number of data in each query. The maximum is 1000, 500 is recommended. Paging can use the time of the last piece of data of the interface as the start time of the interface to query 1000 further back again. If the interface g is 0, then Limit.

🙋 **Can historical data be deleted by time period?**

👉 Historical data cannot be deleted by time period, it can only be deleted all. Deleting the history entry deletes the data. Copy FBox, import box or clear data, historical item data will be deleted.

🙋 **Which method is called in the SDK to obtain historical data points?**

👉 Get history data, the method is GetByChanneIHistoryData, where the monitoring point is hdataItem, and the channel is the channels under it. The query history record is the channel data under the query history entry.

🙋 **The process of registering historical records to obtain historical data?**

👉 A single historical data point, 100 pieces per pack, 100 packs written to flash, 5 times, memory 100 pieces per pack, 100 packs can be stored, each historical data point can store at least 5w pieces of data, at the same time, record the history You can add 100 points to the data point, and it will not be overwritten when it is full.

🙋 **The historical registration is missing data for a period of time?**

👉 The missing data is missing, and the data cannot be retrieved.

🙋 **History registration mechanism \(in the case of a period of 1 second\)?**

👉 There are 5 channels under one history entry, then 5 data will be collected every second, and 100 data will be collected, which requires 20S. Two history entries are also performed at the same time, but they are calculated separately, and each entry is calculated separately, so it is said that the two history entries are performed at the same time, and the collection time of each history entry still needs 20s.

🙋 **The interface for obtaining historical data is for obtaining historical data. The maximum can only be 1,000 pieces of data. If the historical data exceeds 1,000 pieces, how to obtain the remaining data?**

👉 If there is a need to obtain 5000 pieces of historical data for a certain period of time, first call the interface to obtain the data for a certain period of time, and then use the end time of the previous interface query as the start time of the next call of the historical data interface, and so on , Until the 5000 pieces of data are obtained.

## signalr Push <a id="signalr&#x63A8;&#x9001;"></a>

🙋 **Use signalr to get data?**

👉 Obtaining the data on the device is to obtain the data of the monitoring point, and to obtain the value of the monitoring point, it is recommended to use the signalr real-time data push event, the real-time data push event status and value under the dMonUpdateValue message, the event is triggered, the FBox is called to open all the monitoring points Control interface. The first time this interface is called after going online, all current values ​​will be pushed once, followed by the box thread scanning PLC data for changes and reporting to the server for push.

🙋 **Want to know the state of the box at first?**

👉 When connecting to the signalr, you need to open the point. There are 100 boxes that need to call the open point interface 100 times. There is no limit to the open point interface. After the point is successfully opened, the monitoring point data of all online boxes will be pushed again. Now it is The push is one by one. The status of the fbox is judged through the signalr box status change event, and the box number is also pushed when the data is pushed.

🙋 **The box was originally online, but the network cable was disconnected later, but the status of the box was not pushed?**

👉 If you unplug the network cable, the server will not respond so quickly. It needs to wait 2~3 minutes. The server will ping the box if it does not receive the heartbeat of the box within 2 minutes, and then detect it.

🙋 **How to get the status of FBox?**

👉 The state of the Signalr box state change event \(0: unknown 1: connected 2: timed out 3: disconnected\). 0,3 is offline, 1,2 is online, 2 timeout is an intermediate stage, the server will ping the box, there may be no data. It is possible that the signal is very weak.

🙋 **About opening the monitoring point data push interface**

👉 The X-FBox-ClientId parameter under the interface Header must be consistent with the X-FBox-ClientId under the querystring that created the signalr connection. Before listening to the signalr real-time data change event, you need to call the open monitoring point data push interface. The box needs to be called again every time it goes online. If the interface call fails, it needs to be retried. Otherwise, the box is not subscribed, and the monitoring data in the unsubscribed box cannot be pushed.

🙋 **How to reduce the frequency of signalr's data push?**

👉 The box data reporting mechanism is changed and pushed, and the PLC data will be pushed if it changes. You can set the dead value zone and save the traffic mode \(send to the box control\). These two parameters will slow down the push, and the change push is generally not The frequency can be dared to be adjusted only through these two parameters.

🙋 **Data push after the dead zone is set?**

👉 It will be pushed after the difference between the current data and the last data &gt;= the dead value area.

🙋 **If you need to detect multiple boxes at the same time, do you also need to write a lot of listeners:**

👉 No need, if we use our SDK, all online boxes will be opened. If it is a secondary development by yourself, you only need to subscribe to the box you want to detect \(call the monitoring point push control interface\).

🙋 **How to get data regularly?**

👉 Currently signalr push is changed push, MQTT supports timing push.

🙋 **After all the monitoring points are turned on, after the box is suddenly disconnected and re-launched, will all the monitoring points be automatically turned on without any code?**

👉 It needs to be reopened. After the box is offline, the server's subscription information will be cleared. The box is offline, and the opening point needs to be called every time it is online. The opening point only needs to be called once after the box is online.

🙋 **Real-time data push of monitoring points. Normally, there is no state attribute**

👉 It is not available when the plc status is normal. If it is parsed by gson, it will give the default value 0.

🙋 **If the callback function of signalr executes timeout or causes an Exception, when a new data callback is generated, will the callback function not be executed when the received data is executed?**

👉 Try to avoid it and don't process the logic time in the event too long, because the processing time of signalR is limited, which will block signalR, and reconnect after processing it, which means losing data. In theory, the callback function can be executed, but I don't know it all the time. Signalr's processing timeout seems to be 20s. If 20s is not finished, the connection will be retried. For you, it means data loss. This hope can be avoided. If the logic processing time is too long, it is recommended to optimize or use a cache queue. Receiving, unified consumption, to ensure that the callback is not blocked.

🙋 **Will the data pushed by real-time data always be in a timeout state?**

👉 Need to find box technical support to assist customers, the status of the monitoring point is not 0, you need to check the configuration of the client, and check the connection network problem between the plc and the box.

🙋 **What is the cause of the monitoring point status, it will time out for a while, and it will be normal for a while?**

👉 Need to find regional technical support to assist customers. It may be a communication group package. Modify the communication parameters, timeout period and the number of package registers.

🙋 **When the customer develops the program for the second time, do I capture the data of the FlexManager monitoring points?**

👉 These values ​​change in real time. We are triggered by signalr events, not a regular polling mechanism. This data is not stored in our database and cannot be captured.

🙋 **How to update the monitoring point data obtained through signalr to the front-end page?**

👉 We are received by the front-end angular1 framework method. Mvvm mode. You need to research on your own platform. There are roughly two ways to achieve this work: 1. The front-end continuously polls the back-end request data query interface \(no matter whether you use AJAX or what\) and then redraws the returned data on the page, which takes the front-end page as the initiative The way. 2. If the browser supports Websocket, then establish a websocket server in the background, establish a websocket connection with the front-end page, and push from the background to the front-end. After the front-end receives the pushed data, the data is redrawn on the page.

🙋 **Signalr real-time data push and get some monitoring points?**

👉 After the Signalr connection is successful, the online status change event of the box will be triggered, and the point will be opened according to the pushed online box. The data of all current points will be pushed once for the first subscription, and the push will be triggered when the data of the monitoring point changes. If you need to get the data of certain points, just call \(only open the push control interface of certain monitoring points\). Signalr pushes the status of online boxes, deletes online boxes, and does not push the status after adding it, but will push it offline.

🙋 **Is the value of the data pushed by signalr or obtained by the interface different from the value displayed by FlexManager?**

👉 The data pushed is plc data. FlexManager displays the value after the monitoring point is configured with numerical calculation. If you want to push the processed value, you can use edge computing processing at present, and the data processed by edge computing will be consistent.

🙋 **Signalr pushes the data of the monitoring point, and the monitoring point changes and receives two data at a time?**

👉 1. The connection may be established when the instance of New is used. If it is not used later, Start is not closed. Did not put hubProxy.subscribe

```text
The event callback is unsubscribed. When the connectstate+= event is called in c#, -= is required.

  2. There are multiple signalr examples created, and the old objects are not destroyed.
```

🙋**Why the real-time data state pushed by signalr is Normal?**

👉 state is an enumerated type, and Normal represents a normal state.

🙋 **Can only one user account be connected to signalr?**

👉 A single program can be started to connect to multiple signalrs, one account for one signalr, as long as the signalr is connected to the GUID of the opening point of the data push interface. Establish multiple signalr connections with the same account, and expand different box data push interfaces for each signalr. It is recommended that the number of signalr connections is about 1 to 5, with a maximum of 10.

🙋 **The plc and fbox are disconnected, why does the signalr disconnect after a long time?**

👉 Signalr has nothing to do with fbox, signalr is only related to the server, and our server will not detect whether the plc is connected to the box. Signalr is disconnected for a long time because the validity period of the acesstoken interface is two hours. At this time, if you use the original acesstoken to access the server, it is 401. It is necessary to re-obtain the token through refershtoken. The validity period of refershtoken is one month. Moreover, it is useless to refresh the token without reconnecting to the signalr. Without reconnecting, the token in the header is still old. Our server will not judge that you have re-acquired the token and help you replace the original verification. Signalr's internal processing is to ping the server regularly, and token authentication is carried when pinging the server. The signalr reconnection mechanism is to reconnect when the 401 authentication fails when the token expires, and the signalr connection will be disconnected when the network is not good, so the signalr reconnection mechanism should also be handled.

🙋 **signalr push**

👉 The status of the box can be pushed to the client's server, and signalr pushes the status of the box. Our SDK is equivalent to a client with ip when connecting to the server, no need to set . 🙋Open when connecting to signalr, is the data pushed all at once or pushed one by one according to the data points?

👉First of all monitoring points need to be subscribed. After subscribing, all the data is pushed one by one for the first time, and then the changes are pushed. If all the subscribed points change at the same time, all the data will be pushed, if one after another Changes are pushed one by one.

🙋 **Regarding signalr data push and obtaining single data, will it be subcontracted?**

👉 When the program is started, signalr connects and judges whether the box is online. When online, it pushes the data of all monitoring points to the client. After the data of the monitoring points changes, the changed data will be pushed. If you need to get certain data, you can filter it according to boxNo. Subcontracting is also determined by the box.

🙋**Is the data type pushed by Signalr only the String type defined in the document?**

👉The data types of signalr push data include integer, floating point, string, etc.

🙋**500 Internal Server Error is returned when connecting to signalr to push data?**

👉This 500 Internal Server Error is returned when signalr is pushed. There are two cases. Signalr is not connected when the open point interface is called. You can test it first, open signalr locally, and call the open point interface. If there is data push, it means that the signalr connection is successful. of. There is also a situation where the guid of the signalr connection belt is inconsistent with the guid of the open-point interface, which will also cause a 500 Internal Server Error to be returned.

🙋 **Why is the time sent by signalr a messy timestamp? Is the order of sending data consistent with the order of scanning?**

👉The box is a thread that scans the PLC data all the time. It reads one address at a time, but the scanning speed is subtle. The more points, the more time-consuming scanning. This is not necessarily the same. It is limited by various conditions. It is possible that this point cannot be read in the next scan before the box reads the PLC data. Then the box is sent to the server, and then to your program. There are too many influencing factors. .

## Unified Write Value Interface <a id="&#x7EDF;&#x4E00;&#x5199;&#x503C;&#x63A5;&#x53E3;"></a>

🙋 **Get all unified writing group interface:**

👉 is to get all the unified write group parameters.

🙋 **Unified writing group writing interface:**

👉 Rewrite the values of a group of monitoring data uniformly. You can write values to the monitoring groups under different groups. Note: Call the interface to write values to multiple monitoring points under a box, and send them to the box, and the bottom of the box is synchronously written. It is recommended to write values at an interval of 300ms each time. The box writes values to the plc synchronously. The interface only delivers tasks. The boxes register tasks in the queue, and the bottom is written one by one. Too many tasks may cause the writing of values to fail. 

👉 If there are customers who write values uniformly, it is recommended that customers: 1. It is recommended that the customer call the unified write interface every time the write interval is 300ms. 2. Or send the script to the box through the platform edge computing, and the box will perform the unified write operation. 3. Or do processing through plc.

## About the use of the box and platform related issues <a id="&#x5173;&#x4E8E;&#x76D2;&#x5B50;&#x4F7F;&#x7528;&#x53CA;&#x5E73;&#x53F0;&#x76F8;&#x5173;&#x95EE;&#x9898;"></a>

🙋**What does the state of FBox \(0: unknown, 1: connected, 2: timeout, 3: disconnected\) mean?**

👉0,3 status represents the box offline status, 1,2, represents the box online disconnection, timeout is an intermediate segment, the server will ping the box, there may be no data.

🙋**On the FlexManager platform, what is the reason why the firmware version is not displayed in the networking information of the setting box?**

👉After the box is online, the box will be reported to the server. If the client box is not online, it may cause the firmware version information to not be obtained.

🙋 **What is the workflow of the box?**

👉The server and the client are connected through websocket, using the signalR protocol for data push, the server and the box use Tcp/ip long connection to transmit data, and the http interface \(Fbox interface document\) is used to operate the box. The box is connected to the plc, the box has threads to scan data, and the changes are uploaded to the server, and the plc \(control logic processor\) is connected to the device to control the device switch.

🙋 **Is there an open interface for the business process of the copy box?**

👉Process: Re-issue the data of the original box. The interface of the copied box is not open, including the interface of import and export boxes.

🙋 **What function does the replacement box use? Is there an open interface?**

👉 No configuration modification is required to replace the box. The old box will be deleted under the account and can be used after adding it again. The configuration information obtained by the interface remains unchanged. The replacement box does not develop an interface.

🙋**Share box function? Is there a developed interface?**

👉If the customer wants to obtain the data of certain control points through the interface, but can be controlled by the sharing box function on the platform, first share the monitoring points that need to be shared, give the engineer permission, and then add the monitoring points that do not need to be shared to the original On the sharing box of, after adding the box, do not synchronize the monitoring items, otherwise the monitoring points that cannot be shared will be shared. After each sharing, the monitoring point ID of the shared account will be regenerated.

🙋 **Can I always add boxes under an account? Are there any restrictions?**

👉You can always add boxes, but it will affect the response speed of the client. 5000 is recommended.

🙋 **Why do I see sub-address or DB block address in the interface, and why is it not displayed on the platform?**

👉If the word address or DB address is not displayed on the platform, it means that the current register does not support the two addresses.

🙋 **The time of the box, two boxes, the time zone of the data received is different?**

👉There are currently two methods: The box will synchronize the time regularly. The time server is time.fbox360.net. If the box is connected to the Internet via a network cable, you need to open this disconnect, which can be automatically calibrated. When the box is connected to our own server \(including private cloud\), if you use alarm entries or historical data, when the push data finds that the time is inconsistent, it will automatically change the time. In the client, there is a button to force time synchronization, you can try it.

🙋 **There are multiple edge calculations in the client, which are downloaded to the box, and are they executed in parallel or serially?**

👉Download to the box, basically in parallel.

🙋 **How does FBox read PLC data?**

👉The box has a thread to scan the data of the plc device \(millisecond level\), and the changes are uploaded to the server, and the server pushes the client through the signal.

🙋 **Regarding how the box is connected to the device, the attributes of the monitoring point and the device association method?**

👉The box can control the device. Look at the connection between the device and the plc. If there is no case data, just write values ​​to the plc. The attributes of the monitoring points are related to the specific equipment. It is recommended that customers look at our client Flexemanager platform and clear it. When adding the parameters of the monitoring point \(address point table\), look for the equipment party and related personnel \(electrical engineer\) to understand.

🙋 **How many boxes can be added to an account? How many monitoring points can be added to a box?**

👉An account can always be placed in the box, 5000 is recommended, it will not affect the interface push, but it will affect the response speed of the client. The items that can be added for each type of box are different, "Basic Configuration" --&gt; "Data Limit".

🙋 **What measures does FBox have to deal with when the on-site Ethernet cannot be connected to the cloud platform?**

👉Some types of boxes. It can switch freely between 2G and network cable. Sim card and network cable are connected to the Internet at the same time, and the card is given priority. The card has no signal to switch the network cable. The 4G traffic card cannot fix the IP, the server is accessed by the domain name, and the IP may change randomly during maintenance or network type switching.

🙋 **Will the firmware upgrade of the box clear edge computing, and will it affect the distributed scripts?**

👉Updating the firmware will not clear the edge computing. Edge computing is on the FBox and has nothing to do with the server. If the variable plc driver defined in the script is not removed, the script will not be affected.

🙋 **After sharing the box on the client, the browser box list can be immediately known, and the customer also wants to know, is there such a thing?**

👉Sharing is notified. Because it is not universal and this type of change is very large, it is not open. You can restart the box after sharing and receive the online event of the box.

🙋 **About data push on the platform**

👉\(1\): Post push, FBox server calls the configured interface information for data transmission. http basic auth certification.

```text
(2): HTTP post push, the array may contain multiple monitoring points. 137 (the number of successful http requests)/308 (the number of monitored items), 0 (the number of failed http requests)/0 (the number of requested items). When the push has started, add monitoring points without restarting the push service. After disabling the subscription, subscribe The points will be stored in the server group package, and after being enabled again, they will be pushed in sub-packages, with a body length of 200,
```

If the interface call fails, data will be lost.

```text
(3): Post push, the next interface is adjusted after the interface returns, the data is not pushed, the number of times of viewing failures, may be caused by the interface current limit
```

🙋 **About edge computing**

👉There is no interface yet, it needs to be written on the client side. Edge computing has nothing to do with the server and is executed in the box. If you do not remove the variable PLC driver defined in the script, it will not affect the script. For example, if you update the firmware, the script will not be cleared, the box will be offline, and the script will run.

🙋 **The data push of the client after the refresh interval of the data-saving mode entry?**

👉After checking the data saving mode, the data will be pushed according to the entry refresh interval. That is, the start value and the end value of the cycle are different from each other.

🙋 **Dead value zone setting?**

👉Data will be pushed when it reaches the dead zone. That is: difference value &gt;= dead value zone, trigger push.

🙋 **No data for firmware version or data limit**

👉 Boxes that have never been online are displayed, and these data will be reported after the boxes are online.

## SDK Usage Issues <a id="sdk&#x4F7F;&#x7528;&#x95EE;&#x9898;"></a>

🙋**HTTPRequest prompts "Acces-Control-Allow-Origin"**

👉Neither http request nor signalr connection supports cross-domain

🙋**Is the event callback function of C\# SDK Demo single-threaded or multi-threaded?**

👉 It can be regarded as a multi-threaded thread from a fixed thread pool. Signalr has limited processing time and cannot be operated for a long time. Long-time operations are placed in the queue for processing.

🙋**SDK Demo code problem**

👉\(1\). In C\#, sdkdemo is a .net core project.

```text
       Winform is a .net framework project.

       In Java, it is gradle and maven projects.

(2).Signalr needs to maintain a long connection and is a singleton. The Restart() method in the C# SDK only needs to be called once globally, and the internal part of the Restart() method is to obtain the token to connect to the signalr.
```

\(3\) Winform program references SDK, .NET Framework version number must be &gt;=4.6.1, java jdk must be &gt;=1.8.1

\(4\). Call signalr XMLHTTPRequest to prompt "Acces-Control-Allow-Origin"

🙋**The box is shared from other accounts. Is there any event in the SDK to know this action?**

👉No, you can only check whether it is shared from another account through owned and shared parameters.

🙋 **Is the event callback function of the SDK Demo single-threaded or multi-threaded?**

👉It is a thread from a fixed thread pool. It can be treated as a multi-thread, and cannot be operated for a long time, and it can be processed in a queue for a long time.

🙋**C\# SDK introduces dependency package report failed to load file or assembly System .NET HTTP4.1.1?**

👉Cite System.NET HTTP4.3.3 once in the main project and Microsoft.AspNet.SignalR.Client 2.3 in the sub-project

🙋 **Is it necessary to call the restart method in the SDK?**

👉The restart\(\) method is to enter the beginning of the SDK. It is necessary. The restart\(\) opens to enter the SDK, and then operates on a box. Restart can be regarded as initialization, as long as it is called once after construction.

🙋**The following error is reported in the Java Demo interface, indicating that there is a problem with the network of the running machine, and the domain name cannot be resolved?**

👉1.java.net.SocketException: Software caused connection abort: socket write error

```text
 2.Gettokenfailed.javax.net.ssl.SSLHandshakeException: Remote host closed connection during handshake

 3.Get token failed javax.net.UnknownhostExection:account.flexem.cn
```

🙋**Why is it disconnected suddenly after connecting to signalr?**

👉Let the customer try our SDK demo first. Our SDK internally handles signalr and reconnection, and no exception will be reported. After Restart, return to task. Token's runtocompletion is the success state, the internal mechanism of signalr will ping the server, and ping will carry the token

## Other Problems <a id="sdk&#x4F7F;&#x7528;&#x95EE;&#x9898;"></a>

🙋**How to store the data of Fanyi?**

👉Real-time data: Need to add monitoring points, the box must be online \(normal communication with the server\), when the PLC \(equipment\) data changes, the box will report to the server, push through siganlr, real-time data is not stored in the server.

🙋**How many ways do customers get data from us?**

👉1. You save the real-time data pushed through signalr, but the data will be lost when the box is disconnected.

​ 2. Regularly come to our server to obtain historical data. You save it, the box is offline, and the cache of historical data offline is also limited. The more entries, the shorter the storage time, and the space is certain.

​ 3. Obtain real-time data by calling the Obtain Monitoring Point Value Interface. \(Not recommended for use\).

​ 4. Push data through the MQTT protocol.

🙋**Is the communication between FBox and the gateway platform encrypted? Is there anything to deal with in terms of network security?**

👉The DigestAuthentication authentication method is used to connect the Fbox and the server before, and the communication process data is encrypted, and there is integrity check to ensure data security.

🙋**When calling the http interface, the interface is called incorrectly, and the subject does not have a return code?**

👉Api interface request is correct and generally returns 200, 500 is a server error, we return 400 for some common errors, and then put the code in the header. If the call interface parameters are correct or the call fails, it is recommended to use fiddler to check the requested message. Generally, when the box is offline to call the opening point, the interface will return 200, if the box does not exist, it will return 400, and if the signalr is not connected, the interface will return 500 or 421.

🙋**Login failed error in javademo call interface?**

👉The initialization parameter or server address is wrong, and the customer needs to check the writing interface address.

🙋**There are several ways to get the data of Fanyi Box?**

👉1. Private cloud + SDK mode 2. MQTT solution 3. Private cloud + MQTT

🙋**Do I need to set ip to call the interface?**

👉No need to set up, our SDK is equivalent to a client with ip when connecting to the server.

🙋**Is there a monitoring point alarm SMS function here? Is there a charge?**

👉10 SMS or 10 voice messages per day for non-paying user accounts. Paying users can calculate at 0.1 yuan per text message, 0.2 yuan per voice message, and find sales or business for SMS recharge.

🙋**Calling the interface returns 504 \(timeout\)?**

👉Generally, the server is too busy to handle, and the customer provides url for technical support to the SDK.

🙋**How to get the signal of the box?**

👉Get the box signal, you can add local SRW 1022 monitoring point to receive.

🙋**What is an easy-to-use database?**

👉Sqlserver Cassandra \(large throughput\) PG

🙋**What are the OPC Server name and Item name rules?**

👉Corresponding to the box group name, box name, monitoring point group name, and monitoring point name. OPC can only receive real-time data. The internal is to log in to the FBox account, connect to the signalr opening point, and forward the data to the tag

**Note: If the above problems can not help you solve the problem of calling interface and technology, you can add SDK technical support QQ: 3108832390 WeChat ID: FLEXEMSDK \(please add company name, name, and docking sales when adding\) In special circumstances, call the technical support number: 13918456893.**

