# AddHdataDefinitionV2

新增历史条目V2

#### Inheritance

System.Object

AddHdataDefinitionV2

#### Inherited Members

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver.Contract**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_AddHdataDefinitionV2_syntax"></a>

```text
public class AddHdataDefinitionV2 : HdataDtoV2
```

## Constructors <a id="constructors"></a>

### AddHdataDefinitionV2\(\) <a id="FBoxClientDriver_Contract_AddHdataDefinitionV2__ctor"></a>

构造函数

#### Declaration

```text
public AddHdataDefinitionV2()
```

### AddHdataDefinitionV2\(String, Int32, Int32, Int32, Boolean, HDataControlOptionsV2, String, String, Int32, DataType, Int32, DataWidth, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_AddHdataDefinitionV2__ctor_System_String_System_Int32_System_Int32_System_Int32_System_Boolean_FBoxClientDriver_Contract_HDataControlOptionsV2_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public AddHdataDefinitionV2(string name, int recordingPeriod, int integralDigits, int fracDigits, bool isControl, HDataControlOptionsV2 options, string memo, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, int addr, int subAddr, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name | 历史条目名称 |
| System.Int32 | recordingPeriod | 采样时间 |
| System.Int32 | integralDigits | 整数位 |
| System.Int32 | fracDigits | 小数位 |
| System.Boolean | isControl | 是否启用使能设置 |
| [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) | options | 使能设置配置 [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) |
| System.String | memo | 备注 |
| System.String | devAlias | Plc别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型[DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器Id |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 寄存器位宽[DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.Int32 | addr | 主地址 |
| System.Int32 | subAddr | 子地址 |
| System.Int32 | subIndex | DB块地址 |

### AddHdataDefinitionV2\(String, Int32, Int32, Int32, Boolean, HDataControlOptionsV2, String, String, Int32, DataType, String, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_AddHdataDefinitionV2__ctor_System_String_System_Int32_System_Int32_System_Int32_System_Boolean_FBoxClientDriver_Contract_HDataControlOptionsV2_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_String_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public AddHdataDefinitionV2(string name, int recordingPeriod, int integralDigits, int fracDigits, bool isControl, HDataControlOptionsV2 options, string memo, string devAlias, int stationNo, DataType dataType, string regName, int addr, int subAddr, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name | 历史条目名称 |
| System.Int32 | recordingPeriod | 采样时间 |
| System.Int32 | integralDigits | 整数位 |
| System.Int32 | fracDigits | 小数位 |
| System.Boolean | isControl | 是否启用使能设置 |
| [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) | options | 使能设置配置 [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) |
| System.String | memo | 备注 |
| System.String | devAlias | Plc别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型[DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | addr | 主地址 |
| System.Int32 | subAddr | 子地址 |
| System.Int32 | subIndex | DB块地址 |

### AddHdataDefinitionV2\(String, Int32, Int32, Int32, String, String, Int32, DataType, Int32, DataWidth, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_AddHdataDefinitionV2__ctor_System_String_System_Int32_System_Int32_System_Int32_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public AddHdataDefinitionV2(string name, int recordingPeriod, int integralDigits, int fracDigits, string memo, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, int addr, int subAddr, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name | 历史条目名称 |
| System.Int32 | recordingPeriod | 采样时间 |
| System.Int32 | integralDigits | 整数位 |
| System.Int32 | fracDigits | 小数位 |
| System.String | memo | 备注 |
| System.String | devAlias | Plc别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型[DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器Id |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 寄存器位宽[DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.Int32 | addr | 主地址 |
| System.Int32 | subAddr | 子地址 |
| System.Int32 | subIndex | DB块地址 |

### AddHdataDefinitionV2\(String, Int32, Int32, Int32, String, String, Int32, DataType, String, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_AddHdataDefinitionV2__ctor_System_String_System_Int32_System_Int32_System_Int32_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_String_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public AddHdataDefinitionV2(string name, int recordingPeriod, int integralDigits, int fracDigits, string memo, string devAlias, int stationNo, DataType dataType, string regName, int addr, int subAddr, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name | 历史条目名称 |
| System.Int32 | recordingPeriod | 采样时间 |
| System.Int32 | integralDigits | 整数位 |
| System.Int32 | fracDigits | 小数位 |
| System.String | memo | 备注 |
| System.String | devAlias | Plc别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型[DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | addr | 主地址 |
| System.Int32 | subAddr | 子地址 |
| System.Int32 | subIndex | DB块地址 |

