# Alarm Triggering Push

**Listening method name：**`alarmTriggered`

When the alarm entry data triggers an alarm, the server pushes a message. If the alarm condition continues to be met, only the message that triggered the alarm for the first time will be pushed.

**Parameter Correspondence**  


| Filed Name | Type | Description |
| :--- | :--- | :--- |
| boxSessionId | int | Currently negligible |
| values | JSON array | The value collection of the monitoring point, the details of a single attribute are shown in the table below |
| boxUid | string | FBox id |

**Value Corresponding Attributes**

| Filed Name | Type | Description |
| :--- | :--- | :--- |
| id | string | Alarm entry uid |
| value | string | Value |
| state | int | Alarm state，1: Alarm |
| name | string | Alarm entry name |
| msg | string | Alarm information |
| t | int | timestamp of alarm triggering |

**NOTE**：The alarm push does not carry the information of the alarm group. The name of the new alarm entry and the Uid are unique. It is recommended to call the interface to obtain all the alarm entries under the FBox and save them locally, and then find the corresponding alarm group according to the pushed Uid

