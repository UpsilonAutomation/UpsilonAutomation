# SignalR Event

## **SignalR Event** <a id="signalr&#x4E8B;&#x4EF6;"></a>

\*\*\*\*[**Box State Change Event**](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/data-push/untitled-4)\*\*\*\*

This event trigger conditions: 1. This event is triggered when signalr is just connected. Or after the state of the box changes. \(The status represents the connection status of the box and the server\)

\*\*\*\*[**Real-Time Data Push Event**](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/data-push/untitled-3) ****

This event trigger conditions: 1. After receiving the box online event, the open point must be called. 2. The monitoring point data changes. Or the status of the monitoring point changes. \(Status indicates the status of communication between the box and PLC\)

\*\*\*\*[**Alarm Triggered Push** ](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/data-push/untitled-2)\*\*\*\*

This event trigger conditions: 1. When the alarm entry data triggers an alarm condition, the server pushes a message. Note: If the alarm conditions are continuously met, only the message that triggers the alarm for the first time will be pushed.

\*\*\*\*[**Alarm Restore Push** ](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/data-push/untitled-1)\*\*\*\*

This event trigger conditions: 1. When the alarm entry data is restored, the server pushes a message.

## **SignalR Demo** <a id="signalr-demo"></a>

**C\# Demo**

The VS version needs 15.3 and above. C\# demo is a .net core program. The dependency package introduced by Nuget is in the nuget folder of the demo. The framework project requires 4.6 and above to use the dll.

**java Demo**  
The java demo contains Gradle and maven projects, requires java8, and the jar package of signalr is in the repos folder. 

1. After filling in the parameters of the Global.java file 

2. View the README file 

3. Run the jar after compiling

**NOTE：**  
The demos have dealt with the issues of signalr reconnection and token refresh after token expired. 

If you do not use the demo, you need to deal with the reconnection problem after the signalr is disconnected. Each user only needs to create a signalr instance \(singleton\) once globally

You need to handle the expiration of the token yourself, that is, the interface returns 401. Re-login to the interface according to the refresh\_token adjustment and retry the interface after refreshing the access\_token 

The X-FBox-ClientId under the Header in the open point interface should be consistent with the X-FBox-ClientId connected to the signalr, and the guid needs to be newly generated each time the program is started

**After siganlr is disconnected, the data of some boxes will not be pushed**

Each time the signalr is reconnected or the box goes offline, t[he point needs to be adjusted](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/monitoring-point-push-control-interface/untitled-4). The X-FBox-ClientId of the signalr connection must be the same as the X-FBox-ClientId of the open interface The interface may fail or be abnormal. Save the log. The program needs to deal with the open interface exception and retry the mechanism until the interface is successfully called.

**The frequency of siganlr push is too high**

SignalR push is a change push. When PLC data changes, FBox reports to the server. It can be adjusted by setting a dead zone for monitoring points and saving traffic mode.

**The siganlr push data is different from the FlexManager display**

FlexManager is configured with decimal places or numerical calculations, and the pushed data does not process the data reported by the box. If you need to receive push-processed data, you can process it through FlexManager's edge computing

**How to receive data with multiple FBoxes**

The signalr instance must maintain a long connection, and the program is a singleton. To push the current data of the entire FlexManager account, you only need to listen to the real-time data push event and call the open point interface of the online box.

