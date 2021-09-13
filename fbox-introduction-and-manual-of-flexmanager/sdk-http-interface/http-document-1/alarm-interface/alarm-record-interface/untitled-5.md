# Get Alarm Entry State

* **Function Description**

  The interface is used to get the state of the current alarm entry 

* **Request Address** 

   **Old Version \(pick one of two\)**

   **URL1:** `[apiBaseUrl]/v2/box/{boxId}/alarm/defs`  
   **URL2:** `[apiBaseUrl]/v2/box/alarm/defs?boxNo={boxNo}`

   **New Version \(pick one of two\)**

   **URL1:**`[Host Server]/api/v2/box/{boxId}/alarm/defs`

   **URL2:**`[Host Server]/api/v2/box/alarm/defs?boxNo={boxNo}`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxid | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |

* **Request Mode**

   `GET`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   `NULL`

* **Successful Response**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | id | string | Alarm entry Id |
  | code | int | Alarm entry code |
  | name | string | Alarm entry name |
  | boxId | string | Boxid, boxld parameter in Url  |
  | boxNo | string | Box serial number |
  | alarmMsg | string | Alarm content  |
  | alarmState | int | Type, 0：non，1：trigger，2：confirm，3: restore |
  | lastTriggeredTime | dateTime | Triger time  |
  | lastRecoveredTime | dateTime | Restore time |
  | valueOnLastEvent | Object | Value |

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | Execution succeed |
  | 401 | accessToken expired |
  | 404 | Interface does not exist, please check URL |
  | 429 | Access interface frequency is too fast |

