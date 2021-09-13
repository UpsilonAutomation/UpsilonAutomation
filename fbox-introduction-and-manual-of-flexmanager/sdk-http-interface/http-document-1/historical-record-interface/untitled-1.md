# Get Historical Record Entry

* **Function Description**

  The interface is used for users to get historical record entry

* **Request Address** 

   **Old Version \(pick one of two\)**

   **URL1:** `[apiBaseUrl]v2/box/{boxId}/hdataitems`

   **URL2:** `[apiBaseUrl]v2/hdataitems?boxNo={boxNo}`

   **New Version \(pick one of two\)**

   **URL1:** `[Host Server]/api/v2/box/{boxId}/hdataitems`

   **URL2:** `[Host Server]/api/v2/hdataitems?boxNo={boxNo}`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | boxNo | string | FBox serial number |

* **Request Mode**

   `GET`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   `NULL`

* **Successful Response**

  | Filed Name | Type | Description |
  | :--- | :--- | :--- |
  | uid | long | History entry Id |
  | name | string | History entry name |
  | period | int | Collection period \(unit: second\) |
  | boxId | long | Box Id |
  | hasCtrl | bool | Whether to start Enable Setting |
  | ctrl | jobject | Enable setting, see the detailed table of enable setting for details |
  | channels | jarray | Channel settings, see channel configuration table for details |

   **Enable Setting Detailed Table:** 

  | Filed Name | Type | Description |
  | :--- | :--- | :--- |
  | ctrlType | int | Enable itesm 0：OFF enable  1：ON enable |
  | devAlias | string | PLC alias \(device alias in remote download\) |
  | station | int | Station Number |
  | dataType | int | Data type, see [Appendix II](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-1) for details |
  | regId | int | Register Id, used in conjunction with ioWidth to determine the unique register |
  | ioWidth | int | Register bit width, used in conjunction with regId to determine the unique register |
  | regName | string | Register name, can determine the unique register, choose one of the above two parameters |
  | addr | int | Main address |
  | subAddr | int | Sub address |
  | addBlk | int | DB block address |

   **Channel Configuration Table**

  | Filed Name | Type | Description |
  | :--- | :--- | :--- |
  | uid | long | Channel Id |
  | name | string | Channel name  |
  | unit | string | Unit |
  | intDigits | int | Integer bits |
  | fracDigits | int | Decimal bits |
  | desc | string | Description |
  | hasSubAddress | bool | Whether to have a subaddress |
  | hasSubIndex | bool | Whether to have a DB block address |
  | devAlias | string | PLC alias \(device alias in remote download\) |
  | station | int | Station number |
  | dataType | int | Data type, see [Appendix II](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-1) for details |
  | regId | int | Register Id, used in conjunction with ioWidth to determine the unique register |
  | ioWidth | int | Register bit width, used in conjunction with regId to determine the unique register |
  | regName | string | Register name, can determine the unique register, choose one of the above two parameters |
  | addr | int | Main address |
  | subAddr | int | sub address |
  | addBlk | int | DB block address |

* **Return Code**

  |  | Filed Name | Description |
  | :--- | :--- | :--- |
  |  | 200 | Execution succeed |
  |  | 401 | accessToken expired |
  |  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
  |  | 404 | The interface does not exist, please check the URL |
  |  | 429 | Access interface frequency is too fast |

