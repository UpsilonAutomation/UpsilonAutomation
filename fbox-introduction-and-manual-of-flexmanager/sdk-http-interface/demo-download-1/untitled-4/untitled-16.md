# AddDataMonitorDefinitionV2

新增监测点条目属性

#### Inheritance

System.Object

AddDataMonitorDefinitionV2

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

#### Syntax <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionV2_syntax"></a>

```text
public class AddDataMonitorDefinitionV2 : DMonDtoV2
```

## Constructors <a id="constructors"></a>

### AddDataMonitorDefinitionV2\(\) <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionV2__ctor"></a>

无参构造函数

#### Declaration

```text
public AddDataMonitorDefinitionV2()
```

### AddDataMonitorDefinitionV2\(Int64, String, String, Int32, DataType, Int32, DataWidth, Int32, Int32, Int32, Int32, Int32, String, PrivilegeType, Boolean, Single, BitStateLabel, String, EncodeType, StringByteOrder, Int32, Boolean, Int32, DmonValueTransform\) <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionV2__ctor_System_Int64_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_System_String_FBoxClientDriver_Contract_PrivilegeType_System_Boolean_System_Single_FBoxClientDriver_Contract_BitStateLabel_System_String_FBoxClientDriver_Contract_EncodeType_FBoxClientDriver_Contract_StringByteOrder_System_Int32_System_Boolean_System_Int32_FBoxClientDriver_Contract_DmonValueTransform_"></a>

构造函数

#### Declaration

```text
public AddDataMonitorDefinitionV2(long groupId, string name, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, int mainAddress, int subAddress, int subIndex, int integralDigits, int fractionalDigits, string unit, PrivilegeType privilege, bool trafficSaving, float deadValue, BitStateLabel bitStateLabel, string memo, EncodeType encoding, StringByteOrder stringByteOrder, int charCount, bool bitIndexEnabled, int bitIndex, DmonValueTransform dmonValueTransform)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | groupId | 盒子ID |
| System.String | name | 监控点分组名称 |
| System.String | devAlias | PLC设备别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器Id |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 位宽 [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 索引地址（地址块） |
| System.Int32 | integralDigits | 整数位 |
| System.Int32 | fractionalDigits | 小数位 |
| System.String | unit | 单位 |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) | privilege | 读写模式 [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) |
| System.Boolean | trafficSaving | 省流量模式 |
| System.Single | deadValue | 死区值 |
| [BitStateLabel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BitStateLabel.html) | bitStateLabel | 位类型数据标签 [BitStateLabel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BitStateLabel.html) |
| System.String | memo | 备注 |
| [EncodeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EncodeType.html) | encoding | 编码方式 [EncodeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EncodeType.html) |
| [StringByteOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StringByteOrder.html) | stringByteOrder | 字节序 [StringByteOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StringByteOrder.html) |
| System.Int32 | charCount | 字符个数 |
| System.Boolean | bitIndexEnabled | 是否启用按位索引 |
| System.Int32 | bitIndex | 按位索引号 |
| [DmonValueTransform](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DmonValueTransform.html) | dmonValueTransform | 数据运算 |

### AddDataMonitorDefinitionV2\(String, String, String, Int32, DataType, String, Int32, Int32, Int32, Int32, Int32, String, PrivilegeType, Boolean, Single, BitStateLabel, String, EncodeType, StringByteOrder, Int32, Boolean, Int32, DmonValueTransform\) <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionV2__ctor_System_String_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_String_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_System_String_FBoxClientDriver_Contract_PrivilegeType_System_Boolean_System_Single_FBoxClientDriver_Contract_BitStateLabel_System_String_FBoxClientDriver_Contract_EncodeType_FBoxClientDriver_Contract_StringByteOrder_System_Int32_System_Boolean_System_Int32_FBoxClientDriver_Contract_DmonValueTransform_"></a>

构造函数

#### Declaration

```text
public AddDataMonitorDefinitionV2(string groupName, string name, string devAlias, int stationNo, DataType dataType, string regName, int mainAddress, int subAddress, int subIndex, int integralDigits, int fractionalDigits, string unit, PrivilegeType privilege, bool trafficSaving, float deadValue, BitStateLabel bitStateLabel, string memo, EncodeType encoding, StringByteOrder stringByteOrder, int charCount, bool bitIndexEnabled, int bitIndex, DmonValueTransform dmonValueTransform)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | groupName | 监控点分组名称 |
| System.String | name | 监控点名称 |
| System.String | devAlias | PLC设备别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 索引地址（地址块） |
| System.Int32 | integralDigits | 整数位 |
| System.Int32 | fractionalDigits | 小数位 |
| System.String | unit | 单位 |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) | privilege | 读写模式 [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) |
| System.Boolean | trafficSaving | 省流量模式 |
| System.Single | deadValue | 死区值 |
| [BitStateLabel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BitStateLabel.html) | bitStateLabel | 位类型数据标签[BitStateLabel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BitStateLabel.html) |
| System.String | memo | 备注 |
| [EncodeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EncodeType.html) | encoding | 编码方式 [EncodeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EncodeType.html) |
| [StringByteOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StringByteOrder.html) | stringByteOrder | 字节序 [StringByteOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StringByteOrder.html) |
| System.Int32 | charCount | 字符个数 |
| System.Boolean | bitIndexEnabled | 是否启用按位索引 |
| System.Int32 | bitIndex | 按位索引号 |
| [DmonValueTransform](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DmonValueTransform.html) | dmonValueTransform | 数据运算 |

