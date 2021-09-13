# Get Some Monitory Point

* **Function Description**

   This interface can be used for users to obtain certain monitoring points

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL1:**`[apiBaseUrl]v2/box/{boxId}/dmon/get`

   **URL2:**`[apiBaseUrl]v2/box/dmon/get?boxNo={boxNo}`

   **New Version**

   **URL1:**`[Host Server]/api/v2/box/{boxId}/dmon/get`

   **URL2:**`[Host Server]/api/v2/box/dmon/get?boxNo={boxNo}`

* **Address Paramter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxid | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | boxNo | string | FBox serial number |

* **Meader**

   `POST`

* **Header**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

  ```text
  Monitoring point Uid collection 
  ```

* **Successful Response**

   Returns the JSON object of the queried monitoring point collection. The attributes of a single object are as follows:

  <table>
    <thead>
      <tr>
        <th style="text-align:left">Field Name</th>
        <th style="text-align:left">
          <p>Type</p>
          <ul>
            <li>
              <table>
                <thead>
                  <tr>
                    <th style="text-align:left"></th>
                  </tr>
                </thead>
                <tbody></tbody>
              </table>
            </li>
          </ul>
        </th>
        <th style="text-align:left">Description</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="text-align:left">id</td>
        <td style="text-align:left">string</td>
        <td style="text-align:left">Monitoring point id</td>
      </tr>
      <tr>
        <td style="text-align:left">name</td>
        <td style="text-align:left">string</td>
        <td style="text-align:left">Monitoring point name</td>
      </tr>
      <tr>
        <td style="text-align:left">devAlias</td>
        <td style="text-align:left">string</td>
        <td style="text-align:left">Device&apos;s driver alias</td>
      </tr>
      <tr>
        <td style="text-align:left">station</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">PLC communication station number</td>
      </tr>
      <tr>
        <td style="text-align:left">dataType</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">Data type, see <a href="https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/appendix/untitled-1">appendix II</a> for
          details</td>
      </tr>
      <tr>
        <td style="text-align:left">regId</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">Register Id, used in conjunction with ioWidth to determine the unique
          register</td>
      </tr>
      <tr>
        <td style="text-align:left">ioWidth</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">Register bit width, used in conjunction with regId to determine the unique
          register</td>
      </tr>
      <tr>
        <td style="text-align:left">regName</td>
        <td style="text-align:left">string</td>
        <td style="text-align:left">Register name, can determine the unique register, choose one of the above
          two parameters</td>
      </tr>
      <tr>
        <td style="text-align:left">addr</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">PLC main address</td>
      </tr>
      <tr>
        <td style="text-align:left">subAddr</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">PLC sub-address</td>
      </tr>
      <tr>
        <td style="text-align:left">addrBlk</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">PLCDB block address</td>
      </tr>
      <tr>
        <td style="text-align:left">intDigits</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">Integer bit (currently invalid), invalid for bit type, binary, hexadecimal,
          string type</td>
      </tr>
      <tr>
        <td style="text-align:left">fracDigits</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">decimal bits</td>
      </tr>
      <tr>
        <td style="text-align:left">unit</td>
        <td style="text-align:left">string</td>
        <td style="text-align:left">Unit, only valid for word type</td>
      </tr>
      <tr>
        <td style="text-align:left">privilege</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">Read and write mode 2: write-only mode, 4: read-only mode, 6: read-write
          mode</td>
      </tr>
      <tr>
        <td style="text-align:left">trafficSaving</td>
        <td style="text-align:left">boolean</td>
        <td style="text-align:left">Whether to save traffic mode, true: enable, false: not enable</td>
      </tr>
      <tr>
        <td style="text-align:left">deadValue</td>
        <td style="text-align:left">float</td>
        <td style="text-align:left">Dead zone value, data will not be pushed within the range of &#xB1;deadValue</td>
      </tr>
      <tr>
        <td style="text-align:left">label</td>
        <td style="text-align:left">JSON&#x5BF9;&#x8C61;</td>
        <td style="text-align:left">Display label when bit type, attribute ttext: the text displayed when
          the value is 1, ftext: the text displayed when the value is 0</td>
      </tr>
      <tr>
        <td style="text-align:left">memo</td>
        <td style="text-align:left">string</td>
        <td style="text-align:left">Remarks information</td>
      </tr>
      <tr>
        <td style="text-align:left">encoding</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">Encoding format, string type use 0: None, non-string type use, 1: Unicode,
          2: Ascii</td>
      </tr>
      <tr>
        <td style="text-align:left">stringByteOrder</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">String byte order, valid when encoding is in Ascii format 0: reverse order,
          1: forward order</td>
      </tr>
      <tr>
        <td style="text-align:left">charCount</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">Number of strings (only valid for string types)</td>
      </tr>
      <tr>
        <td style="text-align:left">deviceChanged</td>
        <td style="text-align:left">boolean</td>
        <td style="text-align:left">Whether the device is removed (this parameter only appears when removing,
          it is true) This parameter will appear after the FBox connected device
          is changed</td>
      </tr>
      <tr>
        <td style="text-align:left">tstate</td>
        <td style="text-align:left">int</td>
        <td style="text-align:left">Offline task mark, 0: not executed, 1: successful execution, 2: execution
          failed, 3: firmware not supported</td>
      </tr>
      <tr>
        <td style="text-align:left">valueTransform</td>
        <td style="text-align:left">jobject</td>
        <td style="text-align:left">Numerical calculation settings</td>
      </tr>
      <tr>
        <td style="text-align:left">executeOnEdge</td>
        <td style="text-align:left">boolean</td>
        <td style="text-align:left">Whether to enable edge execution, numerical calculation must be configured
          when enabling</td>
      </tr>
    </tbody>
  </table>

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

* **Return Code**

  | Return Code | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see appendix II for details |
  | 404 | The interface does not exist, please check the URL |
  | 429 | Access interface too frequently |

* \*\*\*\*[**The call case is as shown below**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/dmonget.png)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2849%29.png)

