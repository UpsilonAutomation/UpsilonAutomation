# Modify Alarm Entry

* **Function Description**

   The interface is used for users to modify alarm entry

* **Request Address** 

   **Old Version \(pick one of two\)**

   **URL1：**`[apiBaseUrl]v2/box/alarm?boxNo={boxNo}`

   **URL2：**`[apiBaseUrl]v2/box/{boxId}/alarm`

   **New Version \(pick one of two\)**

   **URL1：**`[Host Server]/api/v2/box/alarm?boxNo={boxNo}`

   **URL2：**`[Host Server]/api/v2/box/{boxId}/alarm`

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
   **body为数据监控点列表，JSON格式传输**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | id | string | 报警点条目Id |
  | alarmGrpId | string | 报警点分组Id，若使用alarmGrpId则无需使用dmonGrpName |
  | alarmGrpName | string | 报警点分组名称，若使用alarmGrpName属性则无需使用alarmGrpId属性,若分组不存在，系统自动创建，不能超过15个字符 |
  | condition1 | int | 报警条件一，0：不等于，1：等于，2：大于，3：大于等于，4：小于，5：小于等于 |
  | condtiion2 | int | 报警条件二，0：不等于，1：等于，2：大于，3：大于等于，4：小于，5：小于等于 |
  | operand1 | decimal | 操作数1 |
  | operand2 | deciaml | 操作数2 |
  | condMethod | int | 条件联合，0：无，1：与，2：或 |
  | alarmMsg | string | 报警信息（不要包括test,测试等字样），该参数必填 |
  | memo | string | 备注信息 |
  | devAlias | string | 设备驱动别名 |
  | station | int | PLC通讯站号 |
  | dataType | int | 数据类型，详情见附录二,不支持二进制，十六进制，字符串类型。 |
  | regId | int | 寄存器Id，与ioWidth联合使用，确定唯一寄存器 |
  | ioWidth | int | 寄存器位宽，与regId联合使用，确定唯一寄存器 |
  | regName | string | 寄存器名称，能确定唯一寄存器，与上面两参数任选其一 |
  | addr | int | PLC主地址 |
  | subAddr | int | PLC子地址 |
  | addrBlk | int | PLCDB块地址 |
  | valueTransform | jobject | 数值运算设置 |
  | executeOnEdge | boolean | 是否启用边缘执行，启用时必须配置数值运算 |

 

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

* **Successful Response**

   `NULL`

* **Return Code**

  * | Field Name | Description |
    | :--- | :--- |
    | 200 | Execution succeed  |
    | 401 | accessToken expired |
    | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
    | 429 | Access interface frequency is too fast  |

  |  |
  | :--- |

