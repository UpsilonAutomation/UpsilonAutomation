# Obtain Monitoring Point Value

## `(It is not recommended to use the interface to obtain real-time data!! It is recommended to use singnla to push)` <a id="&#x4E0D;&#x5EFA;&#x8BAE;&#x4F7F;&#x7528;&#x63A5;&#x53E3;&#x83B7;&#x53D6;&#x5B9E;&#x65F6;&#x6570;&#x636E;&#x63A8;&#x8350;&#x4F7F;&#x7528;signalr&#x63A8;&#x9001;"></a>

* **Function Description** This interface can be used for users to obtain monitoring point values. \(There is a frequency limit, it is recommended not to exceed once a second, if it exceeds a certain frequency, IP processing will be blocked\) Obtain real-time data, it is recommended to use [SignalR Push](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/data-push/untitled-3) 
* **Request Address**

  **Old Version：（pick one of two）**

   **URL1：**`[apiBaseUrl]v2/box/{boxId}/dmon/value/get`

   **URL2：**`[apiBaseUrl]v2/dmon/value/get?boxNo={boxNo}`

   **New Version: \(pick one of two\)**

   **URL1：**`[Host Server]/api/v2/box/{boxId}/dmon/value/get`

   **URL2：**`[Host Server]/api/v2/dmon/value/get?boxNo={boxNo}`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in box under boxRegs in [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | boxNo | string | FBox serial number |

* **Request Mode**

   `POST`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | accessToken obtained in "Bearer"+Login Interface |

* **Body**

   JSON object

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | names | jarray | Monitoring point name collection, choose one from ids, use name first, less than 100 elements. |
  | ids | jarray | Monitoring point ID collection, choose one from names, use name first, less than 100 elements. |
  | timeOut | int | Maximum read timeout, null is the default value of the server \(6000ms\) |
  | groupnames | jarray | It is used when there are monitoring points with the same name under different groups. Used in conjunction with the monitoring point name collection, the group name corresponds to the monitoring point name one-to-one |

* **Successful Response**  
   **JSON Array**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | id | string | Monitroing point Id |
  | timestamp | datetime | Timestamp, because the data is pulled from the cache, a timestamp is needed to determine whether it has expired, UTC time |
  | dataType | int | Data type, see [appendix II](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/appendix/untitled-1) |
  | value | object | value |
  | name | string | Monitoring point name |
  | boxId | long | Box Id |
  | status | int | Monitoring point status, 0: normal, 1: no data, 2: timeout, 3: error, 4: Socket exception, 5: FDS error, 16: not completed |
  | connState | int | Box connection status, 0: unknown, 1: connected, 2: timed out, 3: disconnected |
  | connStateTimestamp | datatime | Online time of the box |

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | execution succeed |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see appendix III for details |
  | 404 | The interface does not exist, please check the URL |
  | 429 | Access interface frequency is too fast |

* \*\*\*\*[**The call case is as below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/GetMonitoryPointValue.png)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2836%29.png)

