# UpdateHdataDefinitionV2

更新历史条目实体

#### Inheritance

System.Object

UpdateHdataDefinitionV2

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateHdataDefinitionV2_syntax"></a>

```text
public class UpdateHdataDefinitionV2 : HdataDtoV2
```

## Constructors <a id="constructors"></a>

### UpdateHdataDefinitionV2\(\) <a id="FBoxClientDriver_Contract_UpdateHdataDefinitionV2__ctor"></a>

构造函数

#### Declaration

```text
public UpdateHdataDefinitionV2()
```

### UpdateHdataDefinitionV2\(Int64, String, Int32, Int32, Int32, Boolean, HDataControlOptionsV2, String, String, Int32, DataType, Int32, DataWidth, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_UpdateHdataDefinitionV2__ctor_System_Int64_System_String_System_Int32_System_Int32_System_Int32_System_Boolean_FBoxClientDriver_Contract_HDataControlOptionsV2_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public UpdateHdataDefinitionV2(long id, string name, int recordingPeriod, int integralDigits, int fracDigits, bool isControl, HDataControlOptionsV2 options, string memo, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, int addr, int subAddr, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | id | 历史条目Id |
| System.String | name | 历史条目名称 |
| System.Int32 | recordingPeriod | 采样时间 |
| System.Int32 | integralDigits | 整数位 |
| System.Int32 | fracDigits | 小数位 |
| System.Boolean | isControl | 是否启用使能控制 |
| [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) | options | 使能控制配置[HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) |
| System.String | memo | 备注 |
| System.String | devAlias | Plc别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型[DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器Id |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 寄存器位宽[DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.Int32 | addr | 主地址 |
| System.Int32 | subAddr | 子地址 |
| System.Int32 | subIndex | DB块地址 |

### UpdateHdataDefinitionV2\(Int64, String, Int32, Int32, Int32, Boolean, HDataControlOptionsV2, String, String, Int32, DataType, String, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_UpdateHdataDefinitionV2__ctor_System_Int64_System_String_System_Int32_System_Int32_System_Int32_System_Boolean_FBoxClientDriver_Contract_HDataControlOptionsV2_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_String_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public UpdateHdataDefinitionV2(long id, string name, int recordingPeriod, int integralDigits, int fracDigits, bool isControl, HDataControlOptionsV2 options, string memo, string devAlias, int stationNo, DataType dataType, string regName, int addr, int subAddr, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | id | 历史条目Id |
| System.String | name | 历史条目名称 |
| System.Int32 | recordingPeriod | 采样时间 |
| System.Int32 | integralDigits | 整数位 |
| System.Int32 | fracDigits | 小数位 |
| System.Boolean | isControl | 是否启用使能控制 |
| [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) | options | 使能控制配置[HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) |
| System.String | memo | 备注 |
| System.String | devAlias | Plc别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型[DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | addr | 主地址 |
| System.Int32 | subAddr | 子地址 |
| System.Int32 | subIndex | DB块地址 |

### UpdateHdataDefinitionV2\(Int64, String, Int32, Int32, Int32, String, String, Int32, DataType, Int32, DataWidth, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_UpdateHdataDefinitionV2__ctor_System_Int64_System_String_System_Int32_System_Int32_System_Int32_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public UpdateHdataDefinitionV2(long id, string name, int recordingPeriod, int integralDigits, int fracDigits, string memo, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, int addr, int subAddr, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | id | 历史条目Id |
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

### UpdateHdataDefinitionV2\(Int64, String, Int32, Int32, Int32, String, String, Int32, DataType, String, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_UpdateHdataDefinitionV2__ctor_System_Int64_System_String_System_Int32_System_Int32_System_Int32_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_String_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public UpdateHdataDefinitionV2(long id, string name, int recordingPeriod, int integralDigits, int fracDigits, string memo, string devAlias, int stationNo, DataType dataType, string regName, int addr, int subAddr, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | id | 历史条目Id |
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

## Properties <a id="properties"></a>

### Id <a id="FBoxClientDriver_Contract_UpdateHdataDefinitionV2_Id"></a>

历史记录条目Id

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

