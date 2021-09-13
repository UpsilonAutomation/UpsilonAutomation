# AddAlarmDefinitionV2

新增报警条目参数V2

#### Inheritance

System.Object

AddAlarmDefinitionV2

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

#### Syntax <a id="FBoxClientDriver_Contract_AddAlarmDefinitionV2_syntax"></a>

```text
public class AddAlarmDefinitionV2 : AlarmDefinitionDtoV2
```

## Constructors <a id="constructors"></a>

### AddAlarmDefinitionV2\(\) <a id="FBoxClientDriver_Contract_AddAlarmDefinitionV2__ctor"></a>

无参构造函数

#### Declaration

```text
public AddAlarmDefinitionV2()
```

### AddAlarmDefinitionV2\(String, Int32, DataType, Int32, DataWidth, String, Int32, Int32, Int32, Int64, String, AlarmConditionType, AlarmConditionType, Decimal, Decimal, AlarmConditionCombineMethod, String, Boolean, Int32, String\) <a id="FBoxClientDriver_Contract_AddAlarmDefinitionV2__ctor_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_String_System_Int32_System_Int32_System_Int32_System_Int64_System_String_FBoxClientDriver_Contract_AlarmConditionType_FBoxClientDriver_Contract_AlarmConditionType_System_Decimal_System_Decimal_FBoxClientDriver_Contract_AlarmConditionCombineMethod_System_String_System_Boolean_System_Int32_System_String_"></a>

构造函数

#### Declaration

```text
public AddAlarmDefinitionV2(string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, string regName, int mainAddress, int subAddress, int subIndex, long groupId, string groupName, AlarmConditionType condition1, AlarmConditionType condition2, decimal operand1, decimal operand2, AlarmConditionCombineMethod conditionCombineMethod, string alarmMessage, bool bitIndexEnabled, int bitIndex, string memo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | devAlias | PLC设备别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器ID |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 位宽 [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |
| System.Int64 | groupId | 报警分组ID |
| System.String | groupName | 报警分组名称 |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition1 | 条件一，若选择bit数据类型，bit为ON:条件一EQ [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition2 | 报警条件二 [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| System.Decimal | operand1 | 条件值 |
| System.Decimal | operand2 | 条件值 |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) | conditionCombineMethod | 组合条件关联方式 [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |
| System.String | alarmMessage | 报警消息 |
| System.Boolean | bitIndexEnabled | 是否启用按位索引 |
| System.Int32 | bitIndex | 按位索引号 |
| System.String | memo | 报警备注 |

### AddAlarmDefinitionV2\(String, Int32, DataType, Int32, DataWidth, String, Int32, Int32, Int32, Int64, String, AlarmConditionType, AlarmConditionType, Decimal, Decimal, AlarmConditionCombineMethod, String, String\) <a id="FBoxClientDriver_Contract_AddAlarmDefinitionV2__ctor_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_String_System_Int32_System_Int32_System_Int32_System_Int64_System_String_FBoxClientDriver_Contract_AlarmConditionType_FBoxClientDriver_Contract_AlarmConditionType_System_Decimal_System_Decimal_FBoxClientDriver_Contract_AlarmConditionCombineMethod_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public AddAlarmDefinitionV2(string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, string regName, int mainAddress, int subAddress, int subIndex, long groupId, string groupName, AlarmConditionType condition1, AlarmConditionType condition2, decimal operand1, decimal operand2, AlarmConditionCombineMethod conditionCombineMethod, string alarmMessage, string memo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | devAlias | PLC设备别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器ID |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 位宽 [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |
| System.Int64 | groupId | 报警分组ID |
| System.String | groupName | 报警分组名称 |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition1 | 条件一，若选择bit数据类型，bit为ON:条件一EQ [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition2 | 报警条件二 [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| System.Decimal | operand1 | 条件值 |
| System.Decimal | operand2 | 条件值 |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) | conditionCombineMethod | 组合条件关联方式 [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |
| System.String | alarmMessage | 报警消息 |
| System.String | memo | 报警备注 |

### AddAlarmDefinitionV2\(String, Int32, DataType, Int32, DataWidth, String, Int32, Int32, Int32, Int64, String, AlarmConditionType, Decimal, AlarmConditionCombineMethod, String, Boolean, Int32, String\) <a id="FBoxClientDriver_Contract_AddAlarmDefinitionV2__ctor_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_String_System_Int32_System_Int32_System_Int32_System_Int64_System_String_FBoxClientDriver_Contract_AlarmConditionType_System_Decimal_FBoxClientDriver_Contract_AlarmConditionCombineMethod_System_String_System_Boolean_System_Int32_System_String_"></a>

构造函数

#### Declaration

```text
public AddAlarmDefinitionV2(string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, string regName, int mainAddress, int subAddress, int subIndex, long groupId, string groupName, AlarmConditionType condition1, decimal operand1, AlarmConditionCombineMethod conditionCombineMethod, string alarmMessage, bool bitIndexEnabled, int bitIndex, string memo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | devAlias | PLC设备别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器ID |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 位宽 [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |
| System.Int64 | groupId | 报警分组ID |
| System.String | groupName | 报警分组名称 |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition1 | 条件一，若选择bit数据类型，bit为ON:条件一EQ [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| System.Decimal | operand1 | 条件值 |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) | conditionCombineMethod | 组合条件关联方式 [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |
| System.String | alarmMessage | 报警消息 |
| System.Boolean | bitIndexEnabled | 是否启用按位索引 |
| System.Int32 | bitIndex | 按位索引号 |
| System.String | memo | 报警备注 |

### AddAlarmDefinitionV2\(String, Int32, DataType, Int32, DataWidth, String, Int32, Int32, Int32, Int64, String, AlarmConditionType, Decimal, AlarmConditionCombineMethod, String, String\) <a id="FBoxClientDriver_Contract_AddAlarmDefinitionV2__ctor_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_String_System_Int32_System_Int32_System_Int32_System_Int64_System_String_FBoxClientDriver_Contract_AlarmConditionType_System_Decimal_FBoxClientDriver_Contract_AlarmConditionCombineMethod_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public AddAlarmDefinitionV2(string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, string regName, int mainAddress, int subAddress, int subIndex, long groupId, string groupName, AlarmConditionType condition1, decimal operand1, AlarmConditionCombineMethod conditionCombineMethod, string alarmMessage, string memo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | devAlias | PLC设备别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器ID |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 位宽 [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |
| System.Int64 | groupId | 报警分组ID |
| System.String | groupName | 报警分组名称 |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition1 | 条件一，若选择bit数据类型，bit为ON:条件一EQ [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| System.Decimal | operand1 | 条件值 |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) | conditionCombineMethod | 组合条件关联方式 [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |
| System.String | alarmMessage | 报警消息 |
| System.String | memo | 报警备注 |

### AddAlarmDefinitionV2\(String, String, Int32, DataType, Int32, DataWidth, String, Int32, Int32, Int32, Int64, String, AlarmConditionType, AlarmConditionType, Decimal, Decimal, AlarmConditionCombineMethod, String, Boolean, Int32, String\) <a id="FBoxClientDriver_Contract_AddAlarmDefinitionV2__ctor_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_String_System_Int32_System_Int32_System_Int32_System_Int64_System_String_FBoxClientDriver_Contract_AlarmConditionType_FBoxClientDriver_Contract_AlarmConditionType_System_Decimal_System_Decimal_FBoxClientDriver_Contract_AlarmConditionCombineMethod_System_String_System_Boolean_System_Int32_System_String_"></a>

构造函数

#### Declaration

```text
public AddAlarmDefinitionV2(string name, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, string regName, int mainAddress, int subAddress, int subIndex, long groupId, string groupName, AlarmConditionType condition1, AlarmConditionType condition2, decimal operand1, decimal operand2, AlarmConditionCombineMethod conditionCombineMethod, string alarmMessage, bool bitIndexEnabled, int bitIndex, string memo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name | 报警名称 |
| System.String | devAlias | PLC设备别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器ID |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 位宽 [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |
| System.Int64 | groupId | 报警分组ID |
| System.String | groupName | 报警分组名称 |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition1 | 条件一，若选择bit数据类型，bit为ON:条件一EQ [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition2 | 报警条件二 [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| System.Decimal | operand1 | 条件值 |
| System.Decimal | operand2 | 条件值 |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) | conditionCombineMethod | 组合条件关联方式 [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |
| System.String | alarmMessage | 报警消息 |
| System.Boolean | bitIndexEnabled | 是否启用按位索引 |
| System.Int32 | bitIndex | 按位索引号 |
| System.String | memo | 报警备注 |

### AddAlarmDefinitionV2\(String, String, Int32, DataType, Int32, DataWidth, String, Int32, Int32, Int32, Int64, String, AlarmConditionType, AlarmConditionType, Decimal, Decimal, AlarmConditionCombineMethod, String, String\) <a id="FBoxClientDriver_Contract_AddAlarmDefinitionV2__ctor_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_String_System_Int32_System_Int32_System_Int32_System_Int64_System_String_FBoxClientDriver_Contract_AlarmConditionType_FBoxClientDriver_Contract_AlarmConditionType_System_Decimal_System_Decimal_FBoxClientDriver_Contract_AlarmConditionCombineMethod_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public AddAlarmDefinitionV2(string name, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, string regName, int mainAddress, int subAddress, int subIndex, long groupId, string groupName, AlarmConditionType condition1, AlarmConditionType condition2, decimal operand1, decimal operand2, AlarmConditionCombineMethod conditionCombineMethod, string alarmMessage, string memo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name | 报警名称 |
| System.String | devAlias | PLC设备别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器ID |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 位宽 [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |
| System.Int64 | groupId | 报警分组ID |
| System.String | groupName | 报警分组名称 |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition1 | 条件一，若选择bit数据类型，bit为ON:条件一EQ [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition2 | 报警条件二 [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| System.Decimal | operand1 | 条件值 |
| System.Decimal | operand2 | 条件值 |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) | conditionCombineMethod | 组合条件关联方式 [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |
| System.String | alarmMessage | 报警消息 |
| System.String | memo | 报警备注 |

### AddAlarmDefinitionV2\(String, String, Int32, DataType, Int32, DataWidth, String, Int32, Int32, Int32, Int64, String, AlarmConditionType, Decimal, AlarmConditionCombineMethod, String, Boolean, Int32, String\) <a id="FBoxClientDriver_Contract_AddAlarmDefinitionV2__ctor_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_String_System_Int32_System_Int32_System_Int32_System_Int64_System_String_FBoxClientDriver_Contract_AlarmConditionType_System_Decimal_FBoxClientDriver_Contract_AlarmConditionCombineMethod_System_String_System_Boolean_System_Int32_System_String_"></a>

构造函数

#### Declaration

```text
public AddAlarmDefinitionV2(string name, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, string regName, int mainAddress, int subAddress, int subIndex, long groupId, string groupName, AlarmConditionType condition1, decimal operand1, AlarmConditionCombineMethod conditionCombineMethod, string alarmMessage, bool bitIndexEnabled, int bitIndex, string memo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name | 报警名称 |
| System.String | devAlias | PLC设备别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器ID |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 位宽 [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |
| System.Int64 | groupId | 报警分组ID |
| System.String | groupName | 报警分组名称 |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition1 | 条件一，若选择bit数据类型，bit为ON:条件一EQ [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| System.Decimal | operand1 | 条件值 |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) | conditionCombineMethod | 组合条件关联方式 [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |
| System.String | alarmMessage | 报警消息 |
| System.Boolean | bitIndexEnabled | 是否启用按位索引 |
| System.Int32 | bitIndex | 按位索引号 |
| System.String | memo | 报警备注 |

### AddAlarmDefinitionV2\(String, String, Int32, DataType, Int32, DataWidth, String, Int32, Int32, Int32, Int64, String, AlarmConditionType, Decimal, AlarmConditionCombineMethod, String, String\) <a id="FBoxClientDriver_Contract_AddAlarmDefinitionV2__ctor_System_String_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_String_System_Int32_System_Int32_System_Int32_System_Int64_System_String_FBoxClientDriver_Contract_AlarmConditionType_System_Decimal_FBoxClientDriver_Contract_AlarmConditionCombineMethod_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public AddAlarmDefinitionV2(string name, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, string regName, int mainAddress, int subAddress, int subIndex, long groupId, string groupName, AlarmConditionType condition1, decimal operand1, AlarmConditionCombineMethod conditionCombineMethod, string alarmMessage, string memo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name | 报警名称 |
| System.String | devAlias | PLC设备别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |
| System.Int32 | regId | 寄存器ID |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 位宽 [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |
| System.Int64 | groupId | 报警分组ID |
| System.String | groupName | 报警分组名称 |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition1 | 条件一，若选择bit数据类型，bit为ON:条件一EQ [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |
| System.Decimal | operand1 | 条件值 |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) | conditionCombineMethod | 组合条件关联方式 [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |
| System.String | alarmMessage | 报警消息 |
| System.String | memo | 报警备注 |

