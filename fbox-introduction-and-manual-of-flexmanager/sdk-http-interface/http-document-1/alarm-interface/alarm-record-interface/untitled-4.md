# Get Alarm History

* **Function Description**

   Get the alarm records of FBox alarm points \(all or a certain code\) within a certain period of time \(there is a frequency limit, each IP should not exceed twice a second, if it exceeds a certain frequency, the IP will be blocked by the Ng agent\)

* **Request Address** 

   **Old Version \(pick one of two\)**

   **URL:**`[apiBaseUrl]v2/box/{boxId}/alarm/data`

   **New Version:**

   **URL:**`[Host Server]/api/v2/box/{boxId}/alarm/data`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |

* **Request Mode**

   `GET`

* **Headers**

  |  | Field Name | Type | Description |
  | :--- | :--- | :--- | :--- |
  |  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body** （Request，QueryString）

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | beginTime | long | Start time \(milliseconds\) long type utc timestamp unix epoch |
  | endTime | long | End time \(milliseconds\) long type utc timestamp unix epoch |
  | name | string | The code of the alarm entry, if the full search is not required, this parameter is not required |
  | limit | int | Get the limit of the number of items, the limit of the number of results. Negative value is forward query, it is recommended to use 500 |

* **Successful Response**

   The returned collection is the data within the time period, left-closed and right-opened collection

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | t | string | Timestamp，unix epoch |
  | i | string | Alarm entry Id |
  | a | int | Type, 0：non，1：trigger，2：confirm，3: restore |
  | n | string | Alarm entry code |
  | m | string | Alarm information |
  | v | string | Value |

* **Return Code**

  * | Field Name | Description |
    | :--- | :--- |
    | 200 | Execution succeed  |
    | 401 | accessToken expired |
    | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
    | 429 | Access interface frequency is too fast  |

  |  |
  | :--- |

* \*\*\*\*[**Postman Sample as below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/AddAlarmHistroy.png)\*\*\*\*

![](../../../../../.gitbook/assets/image%20%2856%29.png)

* \*\*\*\*[**The use case is as below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/HistoryAlarm.gif)\*\*\*\*

![](../../../../../.gitbook/assets/image%20%2845%29.png)

