# Get Some Alarm Entry

* **Function Description**

   The interface is used for users to get some alarm entry

* **Request Address** 

   **Old Version \(pick one of two\)**

   **URL1:** `[apiBaseUrl]v2/box/{boxId}/alarm/get`

   **URL2:** `[apiBaseUrl]v2/box/alarm/get?boxNo={boxNo}`

   **New Version \(pick one of two\)**

   **URL1:** `[Host Server]/api/v2/box/{boxId}/alarm/get`

   **URL2:** `[Host Server]/api/v2/box/alarm/get?boxNo={boxNo}`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | boxNo | string | FBox serial number |

* **Request Mode**

   `POST`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   Alarm entry uid collection

* **Successful Response**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | id | string | Alarm entry Id |
  | code | string | Alarm entry code |
  | devAlias | string | Device driver alias |
  | station | int | PLC communication station number |
  | dataType | int | Data type, see [Appendix II ](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-1)for details |
  | regId | int | Register Id, used in conjunction with ioWidth to determine the unique register |
  | ioWidth | int | Register bit width, used in conjunction with regId to determine the unique register |
  | regName | string | Register name, can determine the unique register, choose one of the above two parameters |
  | addr | int | PLC main address |
  | subAddr | int | PLC sub address |
  | addrBlk | int | PLCDB block address |
  | condition1 | int | Alarm condition 1, 0: not equal to, 1: equal to, 2: greater than, 3: greater than or equal to, 4: less than, 5: less than or equal to |
  | condtiion2 | int | Alarm condition 2, 0: not equal to, 1: equal to, 2: greater than, 3: greater than or equal to, 4: less than, 5: less than or equal to |
  | operand1 | decimal | Operand 1 |
  | operand2 | deciaml | Operand 2 |
  | condMethod | int | Conditional union, 0: none, 1: and, 2: or |
  | alarmMsg | string | Alarm information |
  | group | JSON object | Alarm group information, attributes include: id \(group Id\), name \(group name\) |
  | memo | string | Remark information  |
  | deviceChanged | boolean | Whether the device is removed \(this parameter only appears when removing, it is true\) This parameter will appear after the FBox connected device is changed |
  | tstate | int | Offline task mark, 0: not executed, 1: successful execution, 2: execution failed, 3: firmware not supported |
  | valueTransform | jobject | Numerical calculation settings |
  | executeOnEdge | boolean | Whether to enable edge execution, numerical calculation must be configured when enabling |

 

  **Numerical Calculation Setting Detailed Table**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | maxValue | int | Upper limit |
  | minValue | int | Lower limit |
  | scaleMaxValue | int | Upper limit of proportion |
  | scaleMinValue | int | Lower limit of proportion |
  | gain | int | Gain |
  | offset | int | Offset |
  | type | int | 1: scale conversion, 2: zoom |

  **Return Code**

* |  | Field Name | Description |
  | :--- | :--- | :--- |
  |  | 200 | Execution succeed |
  |  | 401 | accessToken expired  |
  |  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
  |  | 404 | Interface does not exist, please check URL |

