# Modify Data Monitoring Point

* **Interface Function**

   This interface is used for users to modify data monitoring point.

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL1：**`[apiBaseUrl]v2/box/{boxId}/dmon`

   **URL2：**`[apiBaseUrl]v2/box/dmon?boxNo={boxNo}`

   **New Version:**

   **URL1：**`[Host Server]/api/v2/box/{boxId}/dmon`

   **URL2：**`[Host Server]/api/v2/box/dmon?boxNo={boxNo}`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | boxNo | string | FBox serial number |

* **Method**

   `POST`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**  
   **The length of one-time collection should not exceed 20**

  Body is a list of data monitoring points, transmitted in JSON format

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | dmonGrpId | string | Monitoring point group Id, if dmonGrpId is used, dmonGrpName is not required |
  | dmonGrpName | string | The name of the monitoring point group. If the dmonGrpName attribute is used, the dmongrpId attribute is not required. If the group does not exist, the system will automatically create it |
  | id | string | monitoring point Id |
  | name | string | monitoring point name |
  | intDigits | int | Integer bit \(currently invalid\), invalid for bit type, binary, hexadecimal, string type |
  | fracDigits | int | decimal bits |
  | unit | string | Word type unit |
  | privilege | int | Read and write mode 2: write-only mode, 4: read-only mode, 6: read-write mode |
  | devAlias | string | device driver name  |
  | station | int | PLC communication station number  |
  | dataType | int | Data type, see [appendix II](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-1) for details |
  | regId | int | Register Id, used in conjunction with ioWidth to determine the unique register |
  | ioWidth | int | Register bit width, used in conjunction with regId to determine the unique register |
  | regName | string | Register name, can determine the unique register, choose one of the above two parameters |
  | addr | int | PLC main address |
  | subAddr | int | PLC sub address |
  | addrBlk | int | PLCDB block address |
  | trafficSaving | boolean | Whether to save traffic mode, true: enable, false: not enable, the string type is invalid deadValue |
  | deadValue | float | Dead zone value, data is not pushed within the range of ±deadValue, string, bit type, hexadecimal, and binary are not supported |
  | label | JSON对象 | Display label when bit type, attribute ttext: the text displayed when the value is 1, ftext: the text displayed when the value is 0 |
  | memo | string | Remarks information |
  | encoding | int | Encoding format, string type use 0: None, non-string type use, 1: Unicode, 2: Ascii |
  | stringByteOrder | int | String byte order, valid when encoding is in Ascii format 0: reverse order, 1: forward order |
  | charCount | int | Number of strings \(only valid for string type\) |
  | bitIndexEnabled | boolean | Whether to enable bitwise indexing |
  | bitIndex | int | bitwise indexing number |
  | valueTransform | jobject | Numerical calculation settings |
  | executeOnEdge | boolean | Whether to enable edge execution, numerical calculation must be configured when enabling |

   **Numercial Caculation Setting Detailed Table:** 

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | maxValue | int | Upper limit |
  | minValue | int | Lower limit |
  | scaleMaxValue | int | Upper  limit of proportion |
  | scaleMinValue | int | Lower limit of proportion |
  | gain | int | Gain |
  | offset | int | Offset |
  | type | int | 1: scale conversion, 2: zoom |

* **Successful Response**

   `NULL`

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [appendix II](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
  | 429 | Access interface frequency is too fast |

