# SerialPortSettingsV1

串口信息

#### Inheritance

System.Object

SerialPortSettingsV1

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

#### Syntax <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_syntax"></a>

```text
public class SerialPortSettingsV1
```

## Properties <a id="properties"></a>

### AssembleIntervalBitReg <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_AssembleIntervalBitReg"></a>

组包位寄存器间隔

#### Declaration

```text
public int AssembleIntervalBitReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### AssembleIntervalWordReg <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_AssembleIntervalWordReg"></a>

组包字寄存器间隔

#### Declaration

```text
public int AssembleIntervalWordReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### BaudRate <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_BaudRate"></a>

波特率

#### Declaration

```text
public int BaudRate { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DataBits <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_DataBits"></a>

数据位

#### Declaration

```text
public int DataBits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ListRead <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_ListRead"></a>

#### Declaration

```text
public bool ListRead { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### MaxList <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_MaxList"></a>

#### Declaration

```text
public int MaxList { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MaxPacketsBitReg <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_MaxPacketsBitReg"></a>

位组包最大寄存器个数

#### Declaration

```text
public int MaxPacketsBitReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MaxPacketsWordReg <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_MaxPacketsWordReg"></a>

字组包最大寄存器个数

#### Declaration

```text
public int MaxPacketsWordReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Parity <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_Parity"></a>

校验位

#### Declaration

```text
public ParityType Parity { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [ParityType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ParityType.html) |  |

### PlcResponseTimeout <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_PlcResponseTimeout"></a>

通讯超时时间

#### Declaration

```text
public int PlcResponseTimeout { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ProtocolInterval <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_ProtocolInterval"></a>

超时参数

#### Declaration

```text
public int ProtocolInterval { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ProtocolTimeout1 <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_ProtocolTimeout1"></a>

协议超时参数1

#### Declaration

```text
public int ProtocolTimeout1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ProtocolTimeout2 <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_ProtocolTimeout2"></a>

协议超时参数2

#### Declaration

```text
public int ProtocolTimeout2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StopBits <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_StopBits"></a>

停止位

#### Declaration

```text
public int StopBits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### WorkingMode <a id="FBoxClientDriver_Contract_SerialPortSettingsV1_WorkingMode"></a>

#### Declaration

```text
public WorkingMode WorkingMode { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [WorkingMode](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.WorkingMode.html) |  |

