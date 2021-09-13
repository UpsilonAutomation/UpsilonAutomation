# Monitoring Point Value Write

* **Function Description**

   This interface is used for users to write data to monitoring points

* **Request Address**

   **Old Version：（pick one of two）**

   **URL1：**`[apiBaseUrl]v2/box/{boxId}/dmon/value`

   **URL2：**`[apiBaseUrl]v2/dmon/value?boxNo={boxNo}`

   **New Version：（pick one of two）**

   **URL1：**`[Host Server]/api/v2/box/{boxId}/dmon/value`

   **URL2：**`[Host Server]/api/v2/dmon/value?boxNo={boxNo}`

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

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | id | string | Monitoring point uid, if id attribute is used, name is not required name |
  | name | string | The name of the monitoring point, no need to use the id attribute if you use name |
  | groupname | string | Monitoring group name, used in conjunction with name, used to distinguish the same name of the monitoring point under different groups |
  | type | int | Value type: {0: value is the type specified in the monitoring point}, {1: value integer is a decimal value, floating-point number and other direct upload} |
  | value | string | value |

  **NOTE:**

* If the value type is 1, all integer types must be converted to decimal integers and sent to the server. The integers with decimal places are first multiplied by 10^n and converted into integers without decimal places.
* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | execution succeed |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see appendix iii for details |
  | 404 | The interface does not exist, please check the URL |
  | 429 | Access interface frequency is too fast |

  **The return code is 200, the box writes the value to the PLC successfully, the return code is 40\*, the box fails to write the value to the PLC**

* \*\*\*\*[**The use case is as shown in the figure below**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/writeValue.gif)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2851%29.png)

