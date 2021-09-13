# New Add Monitoring Point

* **Function Description**

   This interface is used for users to new add data monitoring point.

* **Request address:（ pick one of two）**

  **Old version：**

  **URL:**`[App Server]/api/client/group`

  **New version：**

  **URL:**`[Host Server]/api/client/group`

  \*\*\*\*

* **Address parameter description**

  <table>
    <thead>
      <tr>
        <th style="text-align:left">Parameter Name</th>
        <th style="text-align:left">Type</th>
        <th style="text-align:left">
          <ul>
            <li>
              <table>
                <thead>
                  <tr>
                    <th style="text-align:left">Description</th>
                  </tr>
                </thead>
                <tbody></tbody>
              </table>
            </li>
          </ul>
        </th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="text-align:left">apiBaseUrl</td>
        <td style="text-align:left">string</td>
        <td style="text-align:left">see <a href="https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document">Noun Explaination</a> for
          more details</td>
      </tr>
      <tr>
        <td style="text-align:left">boxId</td>
        <td style="text-align:left">Long</td>
        <td style="text-align:left">the id in the box under the boxRegs in the interface of <a href="https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4">FBox List Obtaining</a>
        </td>
      </tr>
      <tr>
        <td style="text-align:left">boxNo</td>
        <td style="text-align:left">string</td>
        <td style="text-align:left">FBox serial number</td>
      </tr>
    </tbody>
  </table>

* **Request Mode**

   `PUT`

* **Headers**

  | Parameter Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "obtain accessToken in "Bearer"+login interface |

* **Body**

   **The length of one-time collection should not exceed 20**

   Body is a list of data monitoring points, transm

  | Parameter Name | Type | Description |
  | :--- | :--- | :--- |
  | dmonGrpId | string | Monitoring point group Id, if dmonGrpId is used, dmonGrpName is not required |
  | dmonGrpName | string | The name of the monitoring point group. If the dmonGrpName attribute is used, the dmongrpId attribute is not required. If the group does not exist, the system will automatically create it |
  | name | string | Monitoring point name |
  | intDigits | int | Integer bit \(currently invalid\), invalid for bit type, binary, hexadecimal, string type |
  | fracDigits | int | Decimal bits |
  | unit | string | Word type unit |
  | privilege | int | Read and write mode 2: write-only mode, 4: read-only mode, 6: read-write mode |
  | devAlias | string | Device driver alias, please check the alias of "Remote Download" in FlexManager |
  | station | int | PLC communication station number |
  | dataType | int | Data type, see [appendix II](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/appendix/untitled-1) for details |
  | regId | int | Register Id, used in conjunction with ioWidth to determine the unique register |
  | ioWidth | int | Register bit width, used in conjunction with regId to determine the unique register |
  | regName | string | Register name, can determine the unique register, choose one of the above two parameters |
  | addr | int | PLC main address |
  | subAddr | int | PLC sub-address |
  | addrBlk | int | PLCDB block address |
  | trafficSaving | boolean | Whether to save traffic mode, true: enable, false: not enable, the string type is invalid |
  | deadValue | float | Dead zone value, data is not pushed within the range of ±deadValue, string, bit type, hexadecimal, and binary are not supported |
  | label | JSON object | Display label when bit type, attribute ttext: the text displayed when the value is 1, ftext: the text displayed when the value is 0 |
  | memo | string | Remark information |
  | encoding | int | Encoding format, string type use 0: None, non-string type use, 1: Unicode, 2: Ascii |
  | stringByteOrder | int | String byte order, valid when encoding is in Ascii format 0: reverse order, 1: forward order |
  | charCount | int | Number of strings \(only valid for string type |
  | bitIndexEnabled | boolean | Whether to enable bitwise indexing |
  | bitIndex | int | Bitwise index number |
  | valueTransform | jobject | Numerical calculation settings |
  | executeOnEdge | boolean | Whether to enable edge execution, numerical calculation must be configured when enabling |

   **Numerical Calculation Setting Detailed Table**

  | Parameter Name | Type | Description |
  | :--- | :--- | :--- |
  | maxValue | int | Upper limit |
  | minValue | int | Lower limit |
  | scaleMaxValue | int | Upper limit of proportion |
  | scaleMinValue | int | Lower limit of proportion |
  | gain | int | gain |
  | offset | int | offset |
  | type | int | 1: scale conversion, 2: zoom |

* **Successful Response**

   Returns the Id\(long\)List collection of added monitoring points

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | execution succeed |
  | 401 | accessToken expired |
  | 404 | The interface does not exist, please check the URL |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see appendix 3 for details |
  | 429 | Access interface frequency is too fast |

* \*\*\*\*[**Postman Call Sample**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/AddDmon.png)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2838%29.png)

* \*\*\*\*[**The use case is as shown in the figure below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/AddDatamonitoring.gif)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2829%29.png)

