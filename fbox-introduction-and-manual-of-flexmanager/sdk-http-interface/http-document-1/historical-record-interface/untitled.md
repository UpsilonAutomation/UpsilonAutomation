# Get Some Historical Record Entry

* **Function Description**

   The interface is used for users to get some historical record entry

* **Request Address** 

   **Old Version \(pick one of two\)**

   **URL1:** `[apiBaseUrl]v2/box/{boxId}/hdataitems/get`

   **URL2:** `[apiBaseUrl]v2/hdataitems/get?boxNo={boxNo}`

   **New Version \(pick one of two\)**

   **URL1:** `[Host Server]/api/v2/box/{boxId}/hdataitems/get`

   **URL2:**`[Host Server]/api/v2/box/{boxId}/hdataitems/get`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | boxNo | string | FBox serial number |

* **Request Mode**  `POST`
* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | ids | long collection | History record id collection, choose one from names |
  | names | string collection | History record name collection, choose one from Ids |

* **Successful Response**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | uid | long | History record multi-channel Id |
  | name | string | History record multi-channel name |
  | period | int | Collection period \(unit: second\) |
  | boxId | long | Box Id |
  | hasCtrl | bool | Whether to start enable setting |
  | ctrl | JObject | Enable setting, see the detailed table of enable setting for details |
  | channels | JArray | Channel settings, see channel configuration table for details |

   **Enable Configuration Detailed Table** 

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | ctrlType | int | Enable item 0: OFF enable 1: ON enable |
  | devAlias | string | PLC alias \(device alias in remote download\) |
  | station | int | Station number |
  | dataType | int | Data type, see [Appendix II ](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-1)for details |
  | regId | int | Register Id, used in conjunction with ioWidth to determine the unique register |
  | ioWidth | int | Register bit width, used in conjunction with regId to determine the unique register |
  | regName | string | Register name, can determine the unique register, choose one of the above two parameters |
  | addr | int | Main address |
  | subAddr | int | Sub address |
  | addBlk | int | DB block address |
  | valueTransform | jobject | Numerical calculation configuration |
  | executeOnEdge | boolean | Whether to enable edge execution, numerical calculation must be configured when enabling |

   **Numerical Calculation Configuration Detailed Table**

  * | ield Name | Type | Description |
    | :--- | :--- | :--- |
    | maxValue | int | Upper limit |
    | minValue | int | Lower limit |
    | scaleMaxValue | int | Upper limit of proportion |
    | scaleMinValue | int | Lower limit of proportion |
    | gain | int | Gain |
    | offset | int | Offset |
    | type | int | 1: scale conversion, 2: zooM |

  |  |
  | :--- |


  **Channel Configuration Table** 

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | uid | long | Channel Id |
  | name | string | Channel name |
  | unit | string | Unit |
  | intDigits | int | Integer bits |
  | fracDigits | int | Decimal bits |
  | desc | string | Description |
  | hasSubAddress | bool | Whether to have a subaddress |
  | hasSubIndex | bool | Whether to have a DB block address |
  | devAlias | string | PLC alias \(device alias in remote download\) |
  | Station | int | Station number |
  | dataType | int | Data type, see [Appendix II](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-1) for details |
  | regId | int | Register Id, used in conjunction with ioWidth to determine the unique register |
  | ioWidth | int | Register bit width, used in conjunction with regId to determine the unique register |
  | regName | string | Register name, can determine the unique register, choose one of the above two parameters |
  | addr | int | Main address |
  | subAddr | int | sub address |
  | addBlk | int | DB block address |

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | Execution succeed |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
  | 404 | Interface does not exist, please check URL |
  | 429 | Access interface frequency is too fast |

