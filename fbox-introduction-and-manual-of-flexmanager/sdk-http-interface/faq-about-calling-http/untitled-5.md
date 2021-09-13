# Obtain the device's data

1. Log in to the FlexManager software
2. Add the box and make the box online
3. Remote download -&gt; configure the drive device corresponding to the PLC
4. Configure monitoring points \(corresponding to the PLC address point table\)  After completing the above steps, after the communication of the monitoring point in FlexManager is normal, the data can be obtained through the following methods

 **Obtain device data through the following methods**  


**I. Receive via Signalr**

[SignalR ](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/data-push/untitled-5)service，after the signalr is connected, it listens to the boxConnStateChanged event and dMonUpdateValue event. Among them, dMonUpdateValue triggers the premise: it is necessary to [open the online box](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/monitoring-point-push-control-interface/untitled-4)，monitor the point data change or call the open point interface and then push the data

**Note: The demo of signalr is currently available for java and .net,** [**demo download**](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/demo-download-1)\*\*\*\*

