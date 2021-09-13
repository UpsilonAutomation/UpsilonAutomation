# Real-Time Data Push

**前置条件：** 盒子每次上线后均需要调用[开点](https://docs.flexem.net/fbox/zh-cn/tutorials/OpenFBoxAllMonitoryPoint.html)

**Listening method name：**`dMonUpdateValue`  
当监控点数据发生变化或者调用开点时，服务器推送消息。

**参数对应**  


| Filed Name | Type | Description |
| :--- | :--- | :--- |
| boxSessionId | int | 目前可忽略 |
| values | json数组 | 监控点的值集合，单个属性详情见下表 |
| boxUid | string | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |

**value对应属性**

| Filed Name | Type | Description |
| :--- | :--- | :--- |
| id | string | 监控点条目uid |
| name | string | 监控点名称 |
| msg | string | 盒子序列号BoxNo |
| value | string | 值，若条目配置小数位则需程序自己转，服务器不做任何中转 |
| status | int | 如果条目正常，则无此属性，1：无数据，2：超时，3：错误，4：Socket异常，5：FDS错误，16：未完成 |
| t | int | 推送的时间戳\(utc格式\(毫秒\)，监控点数据变化时的时间戳\) |
| gname | string | 分组名称 |

**注：status表示盒子下的监控点与PLC的通讯状态，与PLC通讯正常时，gson解析的status值为0**

