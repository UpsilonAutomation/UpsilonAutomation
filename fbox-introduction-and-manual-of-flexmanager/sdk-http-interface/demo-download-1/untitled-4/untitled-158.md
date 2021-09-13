# UpdateAlarmDefinitonArgs

更新报警条目参数

#### Inheritance

System.Object

UpdateAlarmDefinitonArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_syntax"></a>

```text
public class UpdateAlarmDefinitonArgs
```

## Constructors <a id="constructors"></a>

### UpdateAlarmDefinitonArgs\(\) <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public UpdateAlarmDefinitonArgs()
```

### UpdateAlarmDefinitonArgs\(String, Int64, Int64, Int32, Int32, Int32, Int32, Int32, DataType, DataWidth, AlarmConditionType, AlarmConditionType, Decimal, Decimal, String, AlarmConditionCombineMethod, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs__ctor_System_String_System_Int64_System_Int64_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_FBoxClientDriver_Contract_DataType_FBoxClientDriver_Contract_DataWidth_FBoxClientDriver_Contract_AlarmConditionType_FBoxClientDriver_Contract_AlarmConditionType_System_Decimal_System_Decimal_System_String_FBoxClientDriver_Contract_AlarmConditionCombineMethod_System_Int32_System_Int32_System_Int32_"></a>

多条件触发构造函数

#### Declaration

```text
public UpdateAlarmDefinitonArgs(string boxNo, long alarmDefUid, long alarmGroupUid, int serviceId, int portNo, int stationNo, int deviceId, int regId, DataType dataType, DataWidth regWidth, AlarmConditionType condition1, AlarmConditionType condition2, decimal operand1, decimal operand2, string alarmMessage, AlarmConditionCombineMethod conditionCombineMethod, int mainAddress, int subIndex, int subAddress)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | alarmDefUid | 报警条目UID |
| System.Int64 | alarmGroupUid | 报警组别UID |
| System.Int32 | serviceId | 服务ID |
| System.Int32 | portNo |  |
| System.Int32 | stationNo | 站号 |
| System.Int32 | deviceId | 设备ID |
| System.Int32 | regId | 寄存器ID |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | regWidth | 地址宽度 |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition1 | 条件一，若选择bit数据类型，bit为ON:条件一EQ |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition2 | 条件二 |
| System.Decimal | operand1 | 若选择bit数据类型，bit为ON:条件一为1，bit为OFF:条件一为0 |
| System.Decimal | operand2 | 若选择bit数据类型，条件二为0，若不采用组合条件，条件二传入0 |
| System.String | alarmMessage | 报警信息 |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) | conditionCombineMethod | 组合条件 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subIndex | 子地址索引 |
| System.Int32 | subAddress | 子地址 |

### UpdateAlarmDefinitonArgs\(String, Int64, Int64, Int32, Int32, Int32, Int32, Int32, DataType, DataWidth, AlarmConditionType, Decimal, AlarmConditionCombineMethod, String, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs__ctor_System_String_System_Int64_System_Int64_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_FBoxClientDriver_Contract_DataType_FBoxClientDriver_Contract_DataWidth_FBoxClientDriver_Contract_AlarmConditionType_System_Decimal_FBoxClientDriver_Contract_AlarmConditionCombineMethod_System_String_System_Int32_System_Int32_System_Int32_"></a>

单条件触发构造函数

#### Declaration

```text
public UpdateAlarmDefinitonArgs(string boxNo, long alarmDefUid, long alarmGroupUid, int serviceId, int portNo, int stationNo, int deviceId, int regId, DataType dataType, DataWidth regWidth, AlarmConditionType condition1, decimal operand1, AlarmConditionCombineMethod conditionCombineMethod, string alarmMessage, int mainAddress, int subAddress, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | alarmDefUid | 报警条目UID |
| System.Int64 | alarmGroupUid | 报警组别UID |
| System.Int32 | serviceId | 服务ID |
| System.Int32 | portNo |  |
| System.Int32 | stationNo | 站号 |
| System.Int32 | deviceId | 设备ID |
| System.Int32 | regId | 寄存器ID |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | regWidth | 地址宽度 |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) | condition1 | 条件一，若选择bit数据类型，bit为ON:条件一EQ |
| System.Decimal | operand1 | 若选择bit数据类型，bit为ON:条件一为1，bit为OFF:条件一为0 |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) | conditionCombineMethod | 组合条件 |
| System.String | alarmMessage | 报警信息 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |

## Properties <a id="properties"></a>

### AlarmDefUid <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_AlarmDefUid"></a>

报警条目UID

#### Declaration

```text
public long AlarmDefUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### AlarmGroupUid <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_AlarmGroupUid"></a>

报警组别UID

#### Declaration

```text
public long AlarmGroupUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### AlarmMessage <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_AlarmMessage"></a>

报警信息

#### Declaration

```text
public string AlarmMessage { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxNo <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Condition1 <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_Condition1"></a>

条件一

#### Declaration

```text
public AlarmConditionType Condition1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |  |

### Condition2 <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_Condition2"></a>

条件二

#### Declaration

```text
public AlarmConditionType Condition2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |  |

### ConditionCombineMethod <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_ConditionCombineMethod"></a>

参数连接类型

#### Declaration

```text
public AlarmConditionCombineMethod ConditionCombineMethod { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |  |

### DataType <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_DataType"></a>

数据类型

#### Declaration

```text
public DataType DataType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### DeviceId <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_DeviceId"></a>

设备ID

#### Declaration

```text
public int DeviceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MainAddress <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_MainAddress"></a>

主地址

#### Declaration

```text
public int MainAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Memo <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_Memo"></a>

备注

#### Declaration

```text
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Operand1 <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_Operand1"></a>

操作数一

#### Declaration

```text
public decimal Operand1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Decimal |  |

### Operand2 <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_Operand2"></a>

操作数二

#### Declaration

```text
public decimal Operand2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Decimal |  |

### PortNo <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_PortNo"></a>

#### Declaration

```text
public int PortNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegId <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_RegId"></a>

寄存器ID

#### Declaration

```text
public int RegId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegWidth <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_RegWidth"></a>

地址宽度

#### Declaration

```text
public DataWidth RegWidth { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |  |

### ServiceId <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_ServiceId"></a>

服务ID

#### Declaration

```text
public int ServiceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StationNo <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_StationNo"></a>

站号

#### Declaration

```text
public int StationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubAddress <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_SubAddress"></a>

子地址

#### Declaration

```text
public int SubAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubIndex <a id="FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_SubIndex"></a>

子地址索引

#### Declaration

```text
public int SubIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

