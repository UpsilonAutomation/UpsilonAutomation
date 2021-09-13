# New Add Historical Record

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL1:** `[apiBaseUrl]v2/box/{boxId}/hdataitems`

   **URL2:** `[apiBaseUrl]v2/hdataitems/?boxNo={boxNo}`

   **New Version：**

   **URL1:** `[Host Server]/api/v2/box/{boxId}/hdataitems`

   **URL2:** `[Host Server]/api/v2/hdataitems/?boxNo={boxNo}`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | boxNo | string | FBox serial number |

* **Request Mode**

   `PUT`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   Multi-channel collection of historical records, the record attributes are as follows:

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | name | string | History entry name |
  | period | int | Collection period, unit: second, range 1-86400 |
  | channels | collection | Channel collection, see the table below for individual properties |
  | hasctrl | bool | Whether to use enable, if you need to configure the enable configuration |
  | ctrl | object | Enable configuration properties |

   **Channel Individual Attributes:**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | name | string | Channel name |
  | unit | string | Channel unit |
  | desc | string | Channel description |
  | intDigits | int | Channel integer bits |
  | fracDigits | int | Channel decimal bits |
  | devAlias | string | Device driver alias |
  | station | int | PLC communication station number  |
  | dataType | int | Data type, see [Appendix II](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-1) for details. Binary, hexadecimal, and string types are not supported. |
  | regId | int | Register Id, used in conjunction with ioWidth to determine the unique register |
  | ioWidth | int | Register bit width, used in conjunction with regId to determine the unique register |
  | regName | string | Register name, can determine the unique register, choose one of the above two parameters |
  | addr | int | PLC main address |
  | subAddr | int | PLC sub address  |
  | addrBlk | int | PLCDB block address |
  | valueTransform | jobject | Numerical calculation settings |
  | executeOnEdge | boolean | Whether to enable edge execution, numerical calculation must be configured when enabling |

  **Numerical Calculation Configuration Detailed Table** 

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | maxValue | int | Upper limit |
  | minValue | int | Lower limit |
  | scaleMaxValue | int | Upper limit of proportion |
  | scaleMinValue | int | Lower limit of proportion |
  | gain | int | Gain |
  | offset | int | Offset |
  | type | int | 1: scale conversion, 2: zoom |

   **Enable Configuration Attributes:** 

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | ctrlType | int | Enable item 0: OFF enable 1: ON enable |
  | devAlias | string | PLC alias \(device alias in remote download\) |
  | station | int | Station number |
  | dataType | int | Data type, see [Appendix II](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-1) for details |
  | regId | int | Register Id, used in conjunction with ioWidth to determine the unique register |
  | ioWidth | int | Register bit width, used in conjunction with regId to determine the unique register |
  | regName | string | Register name, can determine the unique register, choose one of the above two parameters |
  | addr | int | Main address |
  | subAddr | int | Sub address |
  | addBlk | int | DB block address |

* **Successful Response**

   Returns the Uid primary key of the added history entry

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | Execution succeed |
  | 401 | accessToken expired |
  | 404 | Interface does not exist, please check URL |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
  | 429 | Access interface frequency is too fast |

* \*\*\*\*[**Postman sample as below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/AddHistory.png)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2848%29.png)

* \*\*\*\*[**The use case is as below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/AddHistory.gif)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2814%29.png)

