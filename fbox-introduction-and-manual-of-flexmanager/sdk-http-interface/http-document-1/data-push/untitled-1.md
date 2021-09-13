# Alarm Recovery Push

**Listening method name：**`alarmRecovered`

When the alarm entry data restores the data, the server pushes a message.

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
| name | string | Alarm entry name |
| msg | string | Alarm information |
| t | int | Time stamp of alarm restoration |

