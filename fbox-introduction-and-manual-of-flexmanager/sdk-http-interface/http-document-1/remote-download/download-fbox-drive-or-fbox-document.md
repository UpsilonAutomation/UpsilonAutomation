# Download FBox Driver

* **Interface Function**

   The driver program for the communication between the box and the PLC will be overwritten. You can call to [get the FBox driver list](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/remote-download/get-fbox-device-list-or-fbox-document), and then splice it to the Body and send it

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL1:** `[apiBaseUrl]v2/box/device?boxNo={boxNo}`

   **URL2:** `[apiBaseUrl]v2/box/{boxId}/device`

   **新版：**

   **URL1:**`[Host Server]/api/v2/box/device?boxNo={boxNo}`

   **URL2:**`[Host Server]/api/v2/box/{boxId}/device`

* **Address Parameter Description**

  


  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxNo | string | FBox serial number |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |

* **Request Mode**

   `POST`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   PLC driver list collection, the parameter attributes of a single drive list are as follows:

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | plcId | int | The ID of the driver. If multiple identical PLCs are mounted under one FBox, the ID is not unique |
  | plcName | string | PLC name |
  | alias | string | PLC alias \(V2 version interface represents equipment through him\) |
  | type | int | 0: serial type，2: network type |
  | advanced | json object | PLC configuration advanced parameters, please refer to the table below for details, if you don’t configure it, you can pass in null. |
  | portNo | int | PLC number, 1: serial port 1, 2: serial port 2, 3: serial port 3, network PLC does not need to be transmitted, the server automatically calculates |
  | interface | int | Serial port parameters, interface type, 0: RS232, 1: RS485\_4, 2: RS485\_2, 85: Network \(Serial port 1 supports RS232, RS485\_2 and RS485\_4, serial port 2 only supports RS485\_2, serial port 3 only supports RS232\) |
  | baudRate | int | Serial port parameters, baud rate |
  | dataBits | int | Serial port parameters, data bits |
  | stopBits | int | Serial port parameters, stop bits |
  | parityType | int | Serial port parameters, parity bits |
  | class | int | 0: master device, 1: slave device, 2: master and slave device \(currently not supported\)） |
  | ip | string | Network PLC parameters, IP address |
  | port | int | Network PLC parameters, port number |
  | enabledBroadcast | boolean | Whether to start the broadcast station number |
  | broadcasetStationNo | int | broadcast station number |
  | slaveNo | int | slave device number |

   **advanced 对象属性：**

  | Field Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | plcResponseTimeout | int | Communication timeout parameter |
  | protocolTimeout1 | int | Protocol timeout parameter 1 |
  | protocolTimeout2 | int | Protocol timeout parameter 2 |
  | maxPacketsWordReg | int | Maximum number of registers in a packet |
  | maxPacketsBitReg | int | Maximum number of registers for bit grouping |
  | assembleIntervalWordReg | int | Packet word register interval |
  | assembleIntervalBitReg | int | Group packet bit register interval |
  | protocolInterval | int | Communication interval time \(unit: s\) |
  | byteOrder16 | int | 16-bit integer byte order 0:21,1:12 |
  | byteOrder32 | int | 32-bit integer byte order 0:4321,1:3412,2:2143,3:1234 |
  | byteOrderFloat | int | 32-bit floating point number section order 0:4321, 1:3412, 2:2143,3:1234 |
  | retryType | int | Retry type, 0: retry, 1: cut off |
  | errMsgDispTime | int | Prompt message duration |

* **Successful Response**

   `NUll`

* **Return Code**

  | Field Name | Parameter Description |
  | :--- | :--- |
  | 200 | Execution success |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2\) for details |
  | 401 | accessToken expired |
  | 404 | The interface does not exist, please check the URL |

* \*\*\*\*[**Postman Sample as Below:** ](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/DownloadDevice.png)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2811%29.png)

* \*\*\*\*[**The use case is as the below:** ](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/downloadDevice.gif)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2816%29.png)

