# UpdateDataMonitorDefinitionV2

更新监控点条目属性

#### Inheritance

System.Object

UpdateDataMonitorDefinitionV2

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionV2_syntax"></a>

```text
public class UpdateDataMonitorDefinitionV2 : DMonDtoV2
```

## Constructors <a id="constructors"></a>

### UpdateDataMonitorDefinitionV2\(\) <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionV2__ctor"></a>

无参构造函数

#### Declaration

```text
public UpdateDataMonitorDefinitionV2()
```

### UpdateDataMonitorDefinitionV2\(Int64, Int64, String, String, Int32, DataType, Int32, DataWidth, Int32, Int32, Int32, Int32, Int32, String, PrivilegeType, Boolean, Single, BitStateLabel, String, EncodeType, StringByteOrder, Int32, Boolean, Int32, DmonValueTransform\) <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionV2__ctor_System_Int64_System_Int64_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_System_String_FBoxClientDriver_Contract_PrivilegeType_System_Boolean_System_Single_FBoxClientDriver_Contract_BitStateLabel_System_String_FBoxClientDriver_Contract_EncodeType_FBoxClientDriver_Contract_StringByteOrder_System_Int32_System_Boolean_System_Int32_FBoxClientDriver_Contract_DmonValueTransform_"></a>

构造函数

#### Declaration

```text
public UpdateDataMonitorDefinitionV2(long id, long groupId, string name, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, int mainAddress, int subAddress, int subIndex, int integralDigits, int fractionalDigits, string unit, PrivilegeType privilege, bool trafficSaving, float deadValue, BitStateLabel bitStateLabel, string memo, EncodeType encoding, StringByteOrder stringByteOrder, int charCount, bool bitIndexEnabled, int bitIndex, DmonValueTransform dmonValueTransform)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | id | 数据监控条目ID |
| System.Int64 | groupId | 监控点组别ID |
| System.String | name | 数据监控条目名称 |
| System.String | devAlias | PLC别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器ID |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 寄存器位宽 [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 索引地址（DB块） |
| System.Int32 | integralDigits | 整数位 |
| System.Int32 | fractionalDigits | 小数位 |
| System.String | unit | 单位 |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) | privilege | 读写模式 [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) |
| System.Boolean | trafficSaving | 省流量模式 |
| System.Single | deadValue | 死区值 |
| [BitStateLabel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BitStateLabel.html) | bitStateLabel | 为类型数据标签 [BitStateLabel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BitStateLabel.html) |
| System.String | memo | 备注 |
| [EncodeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EncodeType.html) | encoding | 字符串类型编码方式 [EncodeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EncodeType.html) |
| [StringByteOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StringByteOrder.html) | stringByteOrder | 字符串类型编码为Ascii时字节序 [StringByteOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StringByteOrder.html) |
| System.Int32 | charCount | 字符串长度 |
| System.Boolean | bitIndexEnabled | 是否启用按位索引 |
| System.Int32 | bitIndex | 按位索引号 |
| [DmonValueTransform](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DmonValueTransform.html) | dmonValueTransform | 数据运算 |

### UpdateDataMonitorDefinitionV2\(Int64, String, String, String, Int32, DataType, String, Int32, Int32, Int32, Int32, Int32, String, PrivilegeType, Boolean, Single, BitStateLabel, String, EncodeType, StringByteOrder, Int32, Boolean, Int32, DmonValueTransform\) <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionV2__ctor_System_Int64_System_String_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_String_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_System_String_FBoxClientDriver_Contract_PrivilegeType_System_Boolean_System_Single_FBoxClientDriver_Contract_BitStateLabel_System_String_FBoxClientDriver_Contract_EncodeType_FBoxClientDriver_Contract_StringByteOrder_System_Int32_System_Boolean_System_Int32_FBoxClientDriver_Contract_DmonValueTransform_"></a>

构造函数

#### Declaration

```text
public UpdateDataMonitorDefinitionV2(long id, string groupName, string name, string devAlias, int stationNo, DataType dataType, string regName, int mainAddress, int subAddress, int subIndex, int integralDigits, int fractionalDigits, string unit, PrivilegeType privilege, bool trafficSaving, float deadValue, BitStateLabel bitStateLabel, string memo, EncodeType encoding, StringByteOrder stringByteOrder, int charCount, bool bitIndexEnabled, int bitIndex, DmonValueTransform dmonValueTransform)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | id | 数据监控条目ID |
| System.String | groupName | 监控点分组名称（若新增的不存在，则新增分组） |
| System.String | name | 监控点名称 |
| System.String | devAlias | PLC别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 索引地址（DB块） |
| System.Int32 | integralDigits | 整数位 |
| System.Int32 | fractionalDigits | 小数位 |
| System.String | unit | 单位 |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) | privilege | 读写模式[PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) |
| System.Boolean | trafficSaving | 省流量模式 |
| System.Single | deadValue | 死区值 |
| [BitStateLabel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BitStateLabel.html) | bitStateLabel | 为类型数据标签[BitStateLabel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BitStateLabel.html) |
| System.String | memo | 备注 |
| [EncodeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EncodeType.html) | encoding | 字符串类型编码方式[EncodeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EncodeType.html) |
| [StringByteOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StringByteOrder.html) | stringByteOrder | 字符串类型编码为Ascii时字节序[StringByteOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StringByteOrder.html) |
| System.Int32 | charCount | 字符串长度 |
| System.Boolean | bitIndexEnabled | 是否启用按位索引 |
| System.Int32 | bitIndex | 按位索引号 |
| [DmonValueTransform](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DmonValueTransform.html) | dmonValueTransform | 数据运算 |

## Properties <a id="properties"></a>

### Id <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionV2_Id"></a>

要更新条目的ID

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

