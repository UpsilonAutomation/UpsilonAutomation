# Get Register Type of Connected Device

* **Interface Function**

   This interface is used to obtain the register attributes of the device connected to the box

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL:**`[apiBaseUrl]device/{deviceId}/spec`

   **New Version：**

   **URL:**`[Host Server]/api/device/{deviceId}/spec`

* **Address Parameter Description**

  |  | Field Name | Type | Parameter Description |
  | :--- | :--- | :--- | :--- |
  |  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  |  | deviceId | int | To get the deviceId of the device, get it from the interface of getting the currently connected device of FBox |

* **Request Mode**

   `GET`

* **Headers**

  | Field Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   `NULL`

* **Return Field** 

  | Field Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | broadcastNo | int | Broadcast station number \(not required\) |
  | byteOrders | json object | Byte order setting object |
  | class | int | Distinguish what station the FBox is used as the device \(the master station is 1\) only the master station needs to be displayed |
  | comPortParams | json object | com port connection settings related parameters \(not required\) |
  | connType | int | Connection method \(serial port network port\) \(not required\) |
  | defaultStationNo | int | Default station number \(the default station number is displayed on the interface\) |
  | ethParams | json object | Network port connection related parameters \(not required\) |
  | id | int | deviceId \(the primary key of the device driver\) |
  | maxStationNo | int | Maximum station number |
  | mfr | string | Equipment manufacturer |
  | minStationNo | int | Minimum station number |
  | name | string | Equipment name |
  | regs | jsonArray | Array of all register information of the device \(a single reg is shown in the table below\) |
  | supportedPlcs | jsonArray | Array of all plc models supported by this driver |

   **Single reg Structure ：**

  | Field Name |  | Type | Parameter Description |
  | :--- | :--- | :--- | :--- |
  | id |  | int | Register id distinguishes the primary key of various registers |
  | name |  | string | Register name |
  | ioWidth |  | int | The width of the data stored in the register |
  | mainAddrType |  | int | Main address type 0: none, 8: octal, 10: decimal, 16: hexadecimal |
  | mainAddrWidth |  | int | Main address width \(not required\) |
  | maxMainAddr |  | int | Maximum primary address |
  | minMainAddr |  | int | Minimum primary address |
  | subAddrType |  | int | Sub address type 0: none, 8: octal, 10: decimal, 16: hexadecimal |
  | subAddrLen |  | int | Sub address range \(\[0,2^subAddrLen -1\]\) |
  | subIndexType |  | int | DB block address type 0: none, 8: octal, 10: decimal, 16: hexadecimal |
  | maxSubIndex |  | int | Maximum DB block address |
  | minSubIndex |  | int | Minimum DB block address |

  **NOTE：**  
   Both the maximum address and the minimum address are decimal numbers, and need to be converted to the hexadecimal number consistent with the address type when displayed.

* **Return Code**

  | Field Name | Parameter Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 404 |  Interface does not exist, please check URL |

