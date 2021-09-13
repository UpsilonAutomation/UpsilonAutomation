# Obtain Monitoring Points according to the Grouping of Monitoring Points

* **Function Description**

   This interface can be used for users to obtain monitoring points according to the grouping of monitoring points

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL:**`[apiBaseUrl]v2/box/{boxId}/dmongroup/{groupId}/dmon`

   **New Version**

   **URL:**`[Host Server]/api/v2/box/{boxId}/dmongroup/{groupId}/dmon`

* **Address Paramter Description**

  | Field Name | Type |  Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | groupId | string | Monitoring point group Id |

* **请求方式**

   `GET`

* **Header**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

   `NULL`

* **Successful Response** 

   **Returns the JSON object of the queried monitoring point collection. The attributes of a single object are as follows:**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | id | string | Monitoring point Id |
  | name | string | Monitoring point name |
  | devAlias | string | Device's drive alias |
  | station | int | PLC communication station number |
  | dataType | int | Data type, see [appendix II](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/appendix/untitled-1) for details |
  | regId | int | Register Id, used in conjunction with ioWidth to determine the unique register |
  | ioWidth | int | Register bit width, used in conjunction with regId to determine the unique register |
  | regName | string | Register name, can determine the unique register, choose one of the above two parameters |
  | addr | int | PLC main address |
  | subAddr | int | PLC sub-address |
  | addrBlk | int | PLCDB block address |
  | intDigits | int | Integer bit \(currently invalid\), invalid for bit type, binary, hexadecimal, string type |
  | fracDigits | int | decimal bits |
  | unit | string | Unit, only valid for word type |
  | privilege | int | Read and write mode 2: write-only mode, 4: read-only mode, 6: read-write mode |
  | trafficSaving | boolean | Whether to save traffic mode, true: enable, false: not enable |
  | deadValue | float | Dead zone value, data will not be pushed within the range of ±deadValue |
  | label | JSON对象 | Display label when bit type, attribute text: the text displayed when the value is 1, ftext: the text displayed when the value is 0 |
  | memo | string | Remarks information |
  | encoding | int | Encoding format, string type use 0: None, non-string type use, 1: Unicode, 2: Ascii |
  | stringByteOrder | int | String byte order, valid when encoding is in Ascii format 0: reverse order, 1: forward order |
  | charCount | int | Number of strings \(only valid for string types\) |
  | deviceChanged | boolean | Whether the device is removed \(this parameter only appears when removing, it is true\) This parameter will appear after the FBox connected device is changed |
  | tstate | int | Offline task mark, 0: not executed, 1: successful execution, 2: execution failed, 3: firmware not supported |

* **Return Code**

  | Return Code | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see appendix III for details |
  | 404 | The interface does not exist, please check the URL |
  | 429 | Access interface too frequently |

