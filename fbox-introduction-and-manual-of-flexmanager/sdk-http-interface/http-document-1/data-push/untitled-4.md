# FBox State Change Push

**Listening method name:**`boxConnStateChanged`  
当服务器侦测到FBox发生状态变更，则会推送消息 消息内容为数组

**The attributes of a single object are as follows：**

| Filed Name | Type | Description |
| :--- | :--- | :--- |
| id | string | FBox Id |
| state | int | The current status of the box, 0: unknown, 1: connected, 2: timed out, 3: disconnected |
| net | int | Box network type 1: Network 2: 2G, 3: 3G \(currently not supported\) 4: WIFI, 5: 4G |
| rssi | int | Signal：0~8 |
| vers | json object | FBox firmware version, fcs, fds, floader. |
| mode | int | FBox status 0: normal, 1: transparent transmission |

**NOTE：** The state value 1 and 2 are both online status, and 0 and 3 are offline status. Call the [opening point](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjDXk75LbPZaPI892sv/http-document-1/monitoring-point-push-control-interface/untitled-4) according to the state

