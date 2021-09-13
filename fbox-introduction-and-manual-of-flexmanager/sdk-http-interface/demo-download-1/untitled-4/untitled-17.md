# AddDataMonitorDefinitionArgs

监测点条目

#### Inheritance

System.Object

AddDataMonitorDefinitionArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_syntax"></a>

```text
public class AddDataMonitorDefinitionArgs
```

## Constructors <a id="constructors"></a>

### AddDataMonitorDefinitionArgs\(\) <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public AddDataMonitorDefinitionArgs()
```

### AddDataMonitorDefinitionArgs\(String, Int64, String, Int32, Int32, Int32, Int32, Int32, DataWidth, Int32, Int32, Int32, DataType, PrivilegeType, Int32, Int32, String\) <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs__ctor_System_String_System_Int64_System_String_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_FBoxClientDriver_Contract_DataWidth_System_Int32_System_Int32_System_Int32_FBoxClientDriver_Contract_DataType_FBoxClientDriver_Contract_PrivilegeType_System_Int32_System_Int32_System_String_"></a>

构造函数

#### Declaration

```text
public AddDataMonitorDefinitionArgs(string boxNo, long dMonGroupUid, string name, int serviceId, int portNo, int stationNo, int deviceId, int regId, DataWidth regWidth, int mainAddress, int subAddress, int subIndex, DataType dataType, PrivilegeType privilegeType, int intDigits, int fracDigits, string unit)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | dMonGroupUid | 监测点组UID |
| System.String | name | 监测点名称 |
| System.Int32 | serviceId | 服务ID 【选择设备：BoxDeviceInfo中获取赋值】 |
| System.Int32 | portNo | 串口1：0，串口2：1，串口3：2，以太网：4096以上 【选择设备：BoxDeviceInfo中获取赋值】 |
| System.Int32 | stationNo | 站号 【输入框输入】 |
| System.Int32 | deviceId | 设备ID 【选择设备：BoxDeviceInfo中获取赋值】 |
| System.Int32 | regId | 寄存器ID 【对应到客户端选择地址类型 DeviceSpecification-RegisterInfo-Id】 |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | regWidth | 地址宽度 【对应到客户端选择地址类型 DeviceSpecification-RegisterInfo-IoWidth】 |
| System.Int32 | mainAddress | 主地址 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-MainAddressType】,8进制 16进制都转换成10进制传入参数,跟PLC有关 |
| System.Int32 | subAddress | 子地址 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-SubAddressType】,8进制 16进制都转换成10进制传入参数,跟PLC有关 |
| System.Int32 | subIndex | 子地址索引 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-SubIndexType】,8进制 16进制都转换成10进制传入参数,跟PLC有关 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 【对用到客户端选择的数据类型 DataType枚举】 |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) | privilegeType | 读写权限 |
| System.Int32 | intDigits | 整数位 |
| System.Int32 | fracDigits | 小数位 |
| System.String | unit | 单位 |

### AddDataMonitorDefinitionArgs\(String, Int64, String, Int32, Int32, Int32, Int32, Int32, DataWidth, Int32, Int32, Int32, DataType, PrivilegeType, String, Int32, Int32, Boolean, Decimal, String\) <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs__ctor_System_String_System_Int64_System_String_System_Int32_System_Int32_System_Int32_System_Int32_System_Int32_FBoxClientDriver_Contract_DataWidth_System_Int32_System_Int32_System_Int32_FBoxClientDriver_Contract_DataType_FBoxClientDriver_Contract_PrivilegeType_System_String_System_Int32_System_Int32_System_Boolean_System_Decimal_System_String_"></a>

构造函数

#### Declaration

```text
public AddDataMonitorDefinitionArgs(string boxNo, long dMonGroupUid, string name, int serviceId, int portNo, int stationNo, int deviceId, int regId, DataWidth regWidth, int mainAddress, int subAddress, int subIndex, DataType dataType, PrivilegeType privilegeType, string desc, int intDigits, int fracDigits, bool trafficSaving, decimal deadZone, string unit)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | dMonGroupUid | 监测点组UID |
| System.String | name | 监测点名称 |
| System.Int32 | serviceId | 服务ID 【选择设备：BoxDeviceInfo中获取赋值】 |
| System.Int32 | portNo | 串口1：0，串口2：1，串口3：2，以太网：4096以上 【选择设备：BoxDeviceInfo中获取赋值】 |
| System.Int32 | stationNo | 站号 【输入框输入】 |
| System.Int32 | deviceId | 设备ID 【选择设备：BoxDeviceInfo中获取赋值】 |
| System.Int32 | regId | 寄存器ID 【对应到客户端选择地址类型 DeviceSpecification-RegisterInfo-Id】 |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | regWidth | 地址宽度 【对应到客户端选择地址类型 DeviceSpecification-RegisterInfo-IoWidth】 |
| System.Int32 | mainAddress | 主地址 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-MainAddressType】,8进制 16进制都转换成10进制传入参数,跟PLC有关 |
| System.Int32 | subAddress | 子地址 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-SubAddressType】,8进制 16进制都转换成10进制传入参数,跟PLC有关 |
| System.Int32 | subIndex | 子地址索引 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-SubIndexType】,8进制 16进制都转换成10进制传入参数,跟PLC有关 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 【对用到客户端选择的数据类型 DataType枚举】 |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) | privilegeType | 读写权限 |
| System.String | desc |  |
| System.Int32 | intDigits | 整数位 |
| System.Int32 | fracDigits | 小数位 |
| System.Boolean | trafficSaving | 省流量模式 |
| System.Decimal | deadZone | 死区值 |
| System.String | unit | 单位 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataType <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_DataType"></a>

数据类型 【对用到客户端选择的数据类型 DataType枚举】

#### Declaration

```text
public DataType DataType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### DeadZone <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_DeadZone"></a>

死区设置值（若有小数位则该死区值的小数位和设置的小数一致，位类型死区值设置为0）

#### Declaration

```text
public decimal DeadZone { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Decimal |  |

### Desc <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_Desc"></a>

描述

#### Declaration

```text
public string Desc { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DeviceId <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_DeviceId"></a>

设备ID 【选择设备：BoxDeviceInfo中获取赋值】

#### Declaration

```text
public int DeviceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DMonGroupUid <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_DMonGroupUid"></a>

监测点组UID

#### Declaration

```text
public long DMonGroupUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### FracDigits <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_FracDigits"></a>

小数位

#### Declaration

```text
public int FracDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IntDigits <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_IntDigits"></a>

整数位

#### Declaration

```text
public int IntDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MainAddress <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_MainAddress"></a>

主地址 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-MainAddressType】,8进制 16进制都转换成10进制传入参数,跟PLC有关 [AddressRadixType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddressRadixType.html)

#### Declaration

```text
public int MainAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Name <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_Name"></a>

监测点名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### PortNo <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_PortNo"></a>

串口1：0，串口2：1，串口3：2，以太网：4096以上 【选择设备：BoxDeviceInfo中获取赋值】

#### Declaration

```text
public int PortNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### PrivilegeType <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_PrivilegeType"></a>

读写权限

#### Declaration

```text
public PrivilegeType PrivilegeType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) |  |

### RegId <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_RegId"></a>

寄存器ID 【对应到客户端选择地址类型 DeviceSpecification-RegisterInfo-Id】

#### Declaration

```text
public int RegId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegWidth <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_RegWidth"></a>

地址宽度 【对应到客户端选择地址类型 DeviceSpecification-RegisterInfo-IoWidth】

#### Declaration

```text
public DataWidth RegWidth { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |  |

### ServiceId <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_ServiceId"></a>

服务ID

#### Declaration

```text
public int ServiceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StationNo <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_StationNo"></a>

站号 【输入框输入】

#### Declaration

```text
public int StationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubAddress <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_SubAddress"></a>

子地址 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-SubAddressType】,8进制 16进制都转换成10进制传入参数,跟PLC有关 [AddressRadixType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddressRadixType.html)

#### Declaration

```text
public int SubAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubIndex <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_SubIndex"></a>

子地址索引 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-SubIndexType】,8进制 16进制都转换成10进制传入参数,跟PLC有关 [AddressRadixType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddressRadixType.html)

#### Declaration

```text
public int SubIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### TrafficSaving <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_TrafficSaving"></a>

省流量模式

#### Declaration

```text
public bool TrafficSaving { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Unit <a id="FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_Unit"></a>

单位

#### Declaration

```text
public string Unit { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

