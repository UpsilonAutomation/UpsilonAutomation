# Get Server Driver List

* **Interface Function**

   Pull the driver supported by FBox from the server

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL:**`[apiBaseUrl]device/spec/{boxType}`

   **New Version：**

   **URL:**`[Host Server]/api/device/spec/{boxType}`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxType | int | FBox type, 0: standard box, 1: mini box, 2: Lite 3: VPN box |

* **Request Mode**

   `GET`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   `NULL`

* **Return Filed** 

  |  | Field Name | Type | Description |
  | :--- | :--- | :--- | :--- |
  |  | id | int | Device Id |
  |  | name | string | PLC name |
  |  | defaultStationNo | int | Default station number |
  |  | minStationNo | int | Minimum station number |
  |  | maxStationNo | int | Maximum station number |
  |  | class | int | Device type, 0: other, 1: master device, 2: slave |
  |  | comPortParams | json object | The default configuration items of the serial port, see the table below for details |
  |  | ethParams | json object | Ethernet default configuration items, see the table below for details |
  |  | byteOrders | json object | Byte order information, see the table below for details |
  |  | supportedPlcs | string array | Supported PLC type |
  |  | regs | JSON array | The list of supported registers, see the table below for details |
  |  | broadcastNo | int | Broadcast number |
  |  | manufacturer | string | PLC manufacture  |
  |  | connType | int | 0: serial port，1: Ethernet |

   **comPortParams Object Attributes：**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | baudRate | int | Serial port baud rate |
  | dataBits | int | Serial port data bits |
  | stopBits | int | Serial port stop bits |
  | parity | int | Serial port parity bits |
  | workingMode | int | Working mode，1:RS232，2:RS485\_4，3:RS485\_2 |
  | plcResponseTimeout | int | Communication timeout time |
  | protocolTimeout1 | int | Protocol timeout parameter 1 |
  | protocolTimeout2 | int | Protocol timeout parameter 2 |
  | maxPacketsWordReg | int | Maximum number of registers in a packet |
  | maxPacketsBitReg | int | Maximum number of registers for bit grouping |
  | assembleIntervalWordReg | int | Packet word register interval |
  | assembleIntervalBitReg | int | Group packet bit register interval |
  | protocolInterval | int | Communication interval time |

   **ethParams Object Attributes：**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | ip | string | Network parameters, IP address |
  | port | int | Communication port |
  | plcResponseTimeout | int | Communication timeout time |
  | protocolTimeout1 | int | Protocol timeout parameter 1 |
  | protocolTimeout2 | int | Protocol timeout parameter 2 |
  | maxPacketsWordReg | int | Maximum number of registers in a packet |
  | maxPacketsBitReg | int | Maximum number of registers for bit grouping |
  | assembleIntervalWordReg | int | Packet word register interval |
  | assembleIntervalBitReg | int | Group packet bit register interval |
  | protocolInterval | int | Communication interval time |

   **regs Array Single Object Attributes：**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | id | int | Register ID, for the same device, this value is not unique, it needs to be combined with Iowidth to determine a register |
  | name | string | Register name  |
  | ioWidth | int | Register bit width，0：Bit,1:Byte,2:Word,3:DWord,4:QWord |
  | mainAddrWitdh | int | Main address addressing mode 0：Bit,1:Byte,2:Word,3:DWord,4:QWord |
  | minMainAddr | int | Minimum primary address value |
  | maxMainAddr | int | Maximum primary address value |
  | mainAddrType | int | Main address hexadecimal type 0: none, 8: octal, 10: decimal, 16: hexadecimal |
  | subAddrType | int | Sub address hexadecimal type 0: none, 8: octal, 10: decimal, 16: hexadecimal |
  | subAddrLen | int | The sub-address is used in the following way: the maximum value of the sub-address is the subAddrLen power of 2 minus 1. If subAddrLen is 3, then the 3rd power of 2 is 8, and the sub-address range is 0-7\( \[0,2^subAddrLen- 1\]\) |
  | subIndexType | int | DB block address hexadecimal type \(generally unique to Siemens\) 0: none, 8: octal, 10: decimal, 16: hexadecimal |
  | minSubIndex | int | Minimum DB block address |
  | maxSubIndex | int | Maximum DB block address |

   **byteOrders Object Attributes：**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | u16 | int | 0:21,1:12 |
  | u32 | int | 0:4321,1:3412,2:2143,3:1234 |
  | float | int | 0:4321,1:3412,2:2143,3:1234 |

* **Return Code**

  | Field Name |  | Description |
  | :--- | :--- | :--- |
  | 401 |  | accessToken expired |
  | 404 |  | The interface does not exist, please check the URL |

