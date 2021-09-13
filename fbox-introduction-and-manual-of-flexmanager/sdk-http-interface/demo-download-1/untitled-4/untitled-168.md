# UpdateHDataDefinitionArgs

更新历史记录条目参数

#### Inheritance

System.Object

UpdateHDataDefinitionArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_syntax"></a>

```text
public class UpdateHDataDefinitionArgs
```

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Control <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_Control"></a>

使能控制参数

#### Declaration

```text
public HDataControl Control { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [HDataControl](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControl.html) |  |

### DataType <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_DataType"></a>

数据类型 【对用到客户端选择的数据类型 DataType枚举】

#### Declaration

```text
public DataType DataType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### Desc <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_Desc"></a>

描述

#### Declaration

```text
public string Desc { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DeviceId <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_DeviceId"></a>

设备ID 【选择设备：BoxDeviceInfo中获取赋值】

#### Declaration

```text
public int DeviceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### FracDigits <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_FracDigits"></a>

小数位

#### Declaration

```text
public int FracDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IntDigits <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_IntDigits"></a>

整数位

#### Declaration

```text
public int IntDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IsControl <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_IsControl"></a>

是否使能控制 true:启用使能控制 false:禁用

#### Declaration

```text
public bool IsControl { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### MainAddress <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_MainAddress"></a>

主地址 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-MainAddressType】,8进制 16进制都转换成10进制传入参数,跟PLC有关

#### Declaration

```text
public int MainAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Name <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_Name"></a>

监控点名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Port <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_Port"></a>

串口1：0，串口2：1，串口3：2，以太网：4096以上 【选择设备：BoxDeviceInfo中获取赋值】

#### Declaration

```text
public int Port { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RecordingPeriod <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_RecordingPeriod"></a>

采集周期 ，最小1s

#### Declaration

```text
public int RecordingPeriod { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegId <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_RegId"></a>

寄存器ID 【对应到客户端选择地址类型 DeviceSpecification-RegisterInfo-Id】

#### Declaration

```text
public int RegId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegWidth <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_RegWidth"></a>

地址宽度 【对应到客户端选择地址类型 DeviceSpecification-RegisterInfo-IoWidth】

#### Declaration

```text
public DataWidth RegWidth { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |  |

### ServiceId <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_ServiceId"></a>

服务ID

#### Declaration

```text
public int ServiceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StationNo <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_StationNo"></a>

站号 【输入框输入】

#### Declaration

```text
public int StationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubAddress <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_SubAddress"></a>

子地址 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-SubAddressType】,8进制 16进制都转换成10进制传入参数,跟PLC有关

#### Declaration

```text
public int SubAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubIndex <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_SubIndex"></a>

子地址索引 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-SubIndexType】,8进制 16进制都转换成10进制传入参数,跟PLC有关

#### Declaration

```text
public int SubIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Uid <a id="FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_Uid"></a>

历史记录条目Uid

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

