# UpdateDataMonitorDefinitionArgs

更新监测点条目参数

#### Inheritance

System.Object

UpdateDataMonitorDefinitionArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_syntax"></a>

```text
public class UpdateDataMonitorDefinitionArgs
```

## Constructors <a id="constructors"></a>

### UpdateDataMonitorDefinitionArgs\(\) <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public UpdateDataMonitorDefinitionArgs()
```

### UpdateDataMonitorDefinitionArgs\(String, Int64, String, Int64, Int32, Int32, Int32, Int32, Int32, Int32, Int32, Int32, DataWidth, DataType, Int32, PrivilegeType, Int32, Int32, String\) <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs__ctor_System_String_System_Int64_System_String_System_Int64_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_FBoxClientDriver_Contract_DataWidth_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_PrivilegeType_System_Int32_System_Int32_System_String_"></a>

构造函数

#### Declaration

```text
public UpdateDataMonitorDefinitionArgs(string boxNo, long dMonUid, string name, long dMonGroupUid, int serviceId, int portNo, int stationNo, int deviceId, int regId, int mainAddress, int subAddress, int subIndex, DataWidth regWidth, DataType dataType, int updateInterval, PrivilegeType privilegeType, int intDigits, int fracDigits, string unit)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | dMonUid | 监测点条目的UID |
| System.String | name | 监测点名称 |
| System.Int64 | dMonGroupUid | 监测点组UID |
| System.Int32 | serviceId | 服务ID |
| System.Int32 | portNo |  |
| System.Int32 | stationNo | 站号 |
| System.Int32 | deviceId | 设备ID |
| System.Int32 | regId | 寄存器ID |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | regWidth | 数据宽度类型 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 |
| System.Int32 | updateInterval | 更新频率 |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) | privilegeType | 读写权限 |
| System.Int32 | intDigits | 整数位 |
| System.Int32 | fracDigits | 小数位 |
| System.String | unit | 单位 |

### UpdateDataMonitorDefinitionArgs\(String, Int64, String, Int64, String, Int32, Int32, Int32, Int32, Int32, Int32, Int32, Int32, DataWidth, DataType, Int32, PrivilegeType, String, Int32, Int32, Boolean, Decimal, String\) <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs__ctor_System_String_System_Int64_System_String_System_Int64_System_String_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_FBoxClientDriver_Contract_DataWidth_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_PrivilegeType_System_String_System_Int32_System_Int32_System_Boolean_System_Decimal_System_String_"></a>

构造函数

#### Declaration

```text
public UpdateDataMonitorDefinitionArgs(string boxNo, long dMonUid, string name, long dMonGroupUid, string dataMonitorDefName, int serviceId, int portNo, int stationNo, int deviceId, int regId, int mainAddress, int subAddress, int subIndex, DataWidth regWidth, DataType dataType, int updateInterval, PrivilegeType privilegeType, string desc, int intDigits, int fracDigits, bool trafficSaving, decimal deadZone, string unit)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | dMonUid | 监测点条目的UID |
| System.String | name | 监测点名称 |
| System.Int64 | dMonGroupUid | 监测点组UID |
| System.String | dataMonitorDefName | 监测点名称 |
| System.Int32 | serviceId | 服务ID |
| System.Int32 | portNo |  |
| System.Int32 | stationNo | 站号 |
| System.Int32 | deviceId | 设备ID |
| System.Int32 | regId | 寄存器ID |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 子地址索引 |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | regWidth | 数据宽度类型 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 |
| System.Int32 | updateInterval | 更新频率 |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) | privilegeType | 读写权限 |
| System.String | desc | 描述 |
| System.Int32 | intDigits | 整数位 |
| System.Int32 | fracDigits | 小数位 |
| System.Boolean | trafficSaving | 省流量模式 |
| System.Decimal | deadZone | 死区值 |
| System.String | unit | 单位 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataMonitorDefName <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_DataMonitorDefName"></a>

监测点名称

#### Declaration

```text
public string DataMonitorDefName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataType <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_DataType"></a>

数据类型

#### Declaration

```text
public DataType DataType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### DeadZone <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_DeadZone"></a>

死区设置值（若有小数位则该死区值的小数位和设置的小数一致，位类型死区值设置为0）

#### Declaration

```text
public decimal DeadZone { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Decimal |  |

### Desc <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_Desc"></a>

描述

#### Declaration

```text
public string Desc { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DeviceId <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_DeviceId"></a>

设备ID

#### Declaration

```text
public int DeviceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DMonGroupUid <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_DMonGroupUid"></a>

监测点组UID

#### Declaration

```text
public long DMonGroupUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### DMonUid <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_DMonUid"></a>

监测点条目的UID

#### Declaration

```text
public long DMonUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### FracDigits <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_FracDigits"></a>

小数位

#### Declaration

```text
public int FracDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IntDigits <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_IntDigits"></a>

整数位

#### Declaration

```text
public int IntDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MainAddress <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_MainAddress"></a>

主地址

#### Declaration

```text
public int MainAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Name <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_Name"></a>

监测点名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### PortNo <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_PortNo"></a>

PortNo

#### Declaration

```text
public int PortNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### PrivilegeType <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_PrivilegeType"></a>

读写权限

#### Declaration

```text
public PrivilegeType PrivilegeType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) |  |

### RegId <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_RegId"></a>

寄存器ID

#### Declaration

```text
public int RegId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegWidth <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_RegWidth"></a>

数据宽度类型

#### Declaration

```text
public DataWidth RegWidth { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |  |

### ServiceId <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_ServiceId"></a>

服务ID

#### Declaration

```text
public int ServiceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StationNo <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_StationNo"></a>

站号

#### Declaration

```text
public int StationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubAddress <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_SubAddress"></a>

子地址

#### Declaration

```text
public int SubAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubIndex <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_SubIndex"></a>

子地址索引

#### Declaration

```text
public int SubIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### TrafficSaving <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_TrafficSaving"></a>

省流量模式

#### Declaration

```text
public bool TrafficSaving { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Unit <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_Unit"></a>

单位

#### Declaration

```text
public string Unit { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### UpdateInterval <a id="FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_UpdateInterval"></a>

更新周期

#### Declaration

```text
public int UpdateInterval { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

