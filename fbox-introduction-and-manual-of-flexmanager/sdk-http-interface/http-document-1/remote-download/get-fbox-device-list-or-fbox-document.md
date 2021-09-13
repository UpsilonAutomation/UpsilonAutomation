# Get FBox Driver List

* **Interface Function**

   This interface can get all the drive devices on the FBox

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL:**`[apiBaseUrl]v2/box/{boxId}/device`

   **New Version：**

   **URL:**`[Host Server]/api/v2/box/{boxId}/device`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | string | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |

* **Request Mode**

   `GET`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   `NULL`

* **Request Field**  
   Return a JSON array, the attributes of a single device are as follows:

  | Field Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | plcId | int | The ID of the PLC. If multiple identical PLCs are mounted under one FBox, the ID is not unique and cannot be used as the primary key |
  | plcName | string | PLC name |
  | alias | string | PLC alias \(V2 version interface represents the device through it\) |
  | type | int | 0: serial port type, 2: network type |
  | advanced | JSON object | PLC configuration advanced parameters, please refer to the following table for details |
  | portNo | int | PLC number, 1: serial port 1, 2: serial port 2, 3: serial port 3, Ethernet above 4096 |
  | plcDongleFlag | int | Remote shutdown status, 0: not supported, 1: enabled, 2: disabled, 3: not configured, 4: box offline |
  | interface | int | Serial port parameters, interface type, 0: RS232, 1: RS485\_2, 2: RS485\_4, 85: Network \(Serial port 1 supports RS232, RS485\_2 and RS485\_4, serial port 2 only supports RS485\_2, serial port 3 only supports RS232\) |
  | baudRate | int | Serial port parameters, baud rate |
  | dataBits | int | Serial port parameters, data bit |
  | stopBits | int | Serial port parameters, stop bits |
  | parityType | int | Serial port parameters, parity bits |
  | class | int | 0: master device, 1: slave device, 2: master and slave device \(currently not supported\) |
  | ip | string | Network PLC parameters, IP address |
  | port | int | Network PLC parameters, port number |
  | enabledBroadcast | boolean | Whether to start the broadcast station number  |
  | broadcasetStationNo | int | broadcast station number  |
  | slaveNo | int | Slave device number |

   **advance Object Attributes：**

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
  | alarmInfDispTms | int | Prompt message duration |

* **Return Code**

  | Return Code | Parameter Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 404 | The interface does not exist, please check the URL |

