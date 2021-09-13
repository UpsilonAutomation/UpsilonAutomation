# BasePlcParameter

基本参数信息

#### Inheritance

System.Object

BasePlcParameter

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

#### Syntax <a id="FBoxClientDriver_Contract_BasePlcParameter_syntax"></a>

```text
public class BasePlcParameter
```

## Properties <a id="properties"></a>

### AlarmInfDispTms <a id="FBoxClientDriver_Contract_BasePlcParameter_AlarmInfDispTms"></a>

提示信息持续时间

#### Declaration

```text
public int AlarmInfDispTms { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### AssembleIntervalBitReg <a id="FBoxClientDriver_Contract_BasePlcParameter_AssembleIntervalBitReg"></a>

组包位寄存器间隔

#### Declaration

```text
public int AssembleIntervalBitReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### AssembleIntervalWordReg <a id="FBoxClientDriver_Contract_BasePlcParameter_AssembleIntervalWordReg"></a>

组包字寄存器间隔

#### Declaration

```text
public int AssembleIntervalWordReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### BroadcastNo <a id="FBoxClientDriver_Contract_BasePlcParameter_BroadcastNo"></a>

广播站号

#### Declaration

```text
public int BroadcastNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DefaultStationNo <a id="FBoxClientDriver_Contract_BasePlcParameter_DefaultStationNo"></a>

默认站号

#### Declaration

```text
public int DefaultStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DriverFileMd5 <a id="FBoxClientDriver_Contract_BasePlcParameter_DriverFileMd5"></a>

驱动文件MD5

#### Declaration

```text
public string DriverFileMd5 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### FloatOrder <a id="FBoxClientDriver_Contract_BasePlcParameter_FloatOrder"></a>

32位浮点数字节序

#### Declaration

```text
public Int32OrFloatOrder FloatOrder { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [Int32OrFloatOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Int32OrFloatOrder.html) |  |

### Id <a id="FBoxClientDriver_Contract_BasePlcParameter_Id"></a>

设备ID

#### Declaration

```text
public int Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Int16Order <a id="FBoxClientDriver_Contract_BasePlcParameter_Int16Order"></a>

16位整数字节序

#### Declaration

```text
public Int16Order Int16Order { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [Int16Order](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Int16Order.html) |  |

### Int32Order <a id="FBoxClientDriver_Contract_BasePlcParameter_Int32Order"></a>

32位整数字节序

#### Declaration

```text
public Int32OrFloatOrder Int32Order { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [Int32OrFloatOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Int32OrFloatOrder.html) |  |

### IsBroadStationNo <a id="FBoxClientDriver_Contract_BasePlcParameter_IsBroadStationNo"></a>

是否启用广播站号

#### Declaration

```text
public bool IsBroadStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### MaxPacketsBitReg <a id="FBoxClientDriver_Contract_BasePlcParameter_MaxPacketsBitReg"></a>

位组包最大寄存器个数

#### Declaration

```text
public int MaxPacketsBitReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MaxPacketsWordReg <a id="FBoxClientDriver_Contract_BasePlcParameter_MaxPacketsWordReg"></a>

字组包最大寄存器个数

#### Declaration

```text
public int MaxPacketsWordReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MaxStationNo <a id="FBoxClientDriver_Contract_BasePlcParameter_MaxStationNo"></a>

最大站号

#### Declaration

```text
public int MaxStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Mfr <a id="FBoxClientDriver_Contract_BasePlcParameter_Mfr"></a>

厂家

#### Declaration

```text
public string Mfr { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### MinStationNo <a id="FBoxClientDriver_Contract_BasePlcParameter_MinStationNo"></a>

最小站号

#### Declaration

```text
public int MinStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Name <a id="FBoxClientDriver_Contract_BasePlcParameter_Name"></a>

PLC名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### PlcResponseTimeout <a id="FBoxClientDriver_Contract_BasePlcParameter_PlcResponseTimeout"></a>

通讯超市时间

#### Declaration

```text
public int PlcResponseTimeout { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### PlcType <a id="FBoxClientDriver_Contract_BasePlcParameter_PlcType"></a>

#### Declaration

```text
public PlcType PlcType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PlcType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcType.html) |  |

### ProtocolInterval <a id="FBoxClientDriver_Contract_BasePlcParameter_ProtocolInterval"></a>

协议超时

#### Declaration

```text
public int ProtocolInterval { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ProtocolTimeout1 <a id="FBoxClientDriver_Contract_BasePlcParameter_ProtocolTimeout1"></a>

协议超时参数1

#### Declaration

```text
public int ProtocolTimeout1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ProtocolTimeout2 <a id="FBoxClientDriver_Contract_BasePlcParameter_ProtocolTimeout2"></a>

协议超时参数2

#### Declaration

```text
public int ProtocolTimeout2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RetryCount <a id="FBoxClientDriver_Contract_BasePlcParameter_RetryCount"></a>

重试次数

#### Declaration

```text
public int RetryCount { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RetryType <a id="FBoxClientDriver_Contract_BasePlcParameter_RetryType"></a>

重试类型

#### Declaration

```text
public RetryType RetryType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [RetryType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RetryType.html) |  |

### SupportedPlcs <a id="FBoxClientDriver_Contract_BasePlcParameter_SupportedPlcs"></a>

支持的PLC

#### Declaration

```text
public IList SupportedPlcs { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.String&gt; |  |

