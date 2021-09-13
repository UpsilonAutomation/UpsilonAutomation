# PlcAdvancedSettings

高级设置

#### Inheritance

System.Object

PlcAdvancedSettings

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

#### Syntax <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_syntax"></a>

```text
public class PlcAdvancedSettings
```

## Properties <a id="properties"></a>

### AlarmInfDispTms <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_AlarmInfDispTms"></a>

提示信息持续时间

#### Declaration

```text
public int AlarmInfDispTms { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### AssembleIntervalBitReg <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_AssembleIntervalBitReg"></a>

组包位寄存器间隔

#### Declaration

```text
public int AssembleIntervalBitReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### AssembleIntervalWordReg <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_AssembleIntervalWordReg"></a>

组包字寄存器间隔

#### Declaration

```text
public int AssembleIntervalWordReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ByteOrder16 <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_ByteOrder16"></a>

16位整数字节序 0:21,1:12

#### Declaration

```text
public U16ByteOrders ByteOrder16 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [U16ByteOrders](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.U16ByteOrders.html) |  |

### ByteOrder32 <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_ByteOrder32"></a>

32位整数字节序 0:4321,1:3412,2:2143,3:1234

#### Declaration

```text
public U32ByteOrders ByteOrder32 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [U32ByteOrders](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.U32ByteOrders.html) |  |

### ByteOrderFloat <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_ByteOrderFloat"></a>

32位浮点数字节序 0:4321,1:3412,2:2143,3:1234

#### Declaration

```text
public U32ByteOrders ByteOrderFloat { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [U32ByteOrders](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.U32ByteOrders.html) |  |

### ErrMsgDispTime <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_ErrMsgDispTime"></a>

#### Declaration

```text
public int ErrMsgDispTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MaxPacketsBitReg <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_MaxPacketsBitReg"></a>

位组包最大寄存器个数

#### Declaration

```text
public int MaxPacketsBitReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MaxPacketsWordReg <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_MaxPacketsWordReg"></a>

字组包最大寄存器个数

#### Declaration

```text
public int MaxPacketsWordReg { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### PlcResponseTimeout <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_PlcResponseTimeout"></a>

通讯超时参数

#### Declaration

```text
public int PlcResponseTimeout { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ProtocolInterval <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_ProtocolInterval"></a>

通讯间隔时间（单位：s）

#### Declaration

```text
public int ProtocolInterval { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ProtocolTimeout1 <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_ProtocolTimeout1"></a>

协议超时参数1

#### Declaration

```text
public int ProtocolTimeout1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ProtocolTimeout2 <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_ProtocolTimeout2"></a>

协议超时参数2

#### Declaration

```text
public int ProtocolTimeout2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RetryCount <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_RetryCount"></a>

重试次数

#### Declaration

```text
public int RetryCount { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RetryType <a id="FBoxClientDriver_Contract_PlcAdvancedSettings_RetryType"></a>

重试类型

#### Declaration

```text
public RetryType RetryType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [RetryType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RetryType.html) |  |

