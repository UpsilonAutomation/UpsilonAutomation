# PlcDevice

#### Inheritance

System.Object

PlcDevice

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

#### Syntax <a id="FBoxClientDriver_Contract_PlcDevice_syntax"></a>

## Properties <a id="properties"></a>

### BroadcastNo <a id="FBoxClientDriver_Contract_PlcDevice_BroadcastNo"></a>

默认广播站号

#### Declaration

```text
public int BroadcastNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ByteOrderSettings <a id="FBoxClientDriver_Contract_PlcDevice_ByteOrderSettings"></a>

#### Declaration

```text
[JsonProperty("byteOrders")]
public ByteOrderSettings ByteOrderSettings { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [ByteOrderSettings](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ByteOrderSettings.html) |  |

### Class <a id="FBoxClientDriver_Contract_PlcDevice_Class"></a>

设备类型

#### Declaration

```text
public DeviceClass Class { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DeviceClass](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DeviceClass.html) |  |

### DefaultStationNo <a id="FBoxClientDriver_Contract_PlcDevice_DefaultStationNo"></a>

默认站号

#### Declaration

```text
public int DefaultStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DeviceConnectionType <a id="FBoxClientDriver_Contract_PlcDevice_DeviceConnectionType"></a>

#### Declaration

```text
[JsonProperty("connType")]
public DeviceConnectionType DeviceConnectionType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DeviceConnectionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DeviceConnectionType.html) |  |

### EthernetSettings <a id="FBoxClientDriver_Contract_PlcDevice_EthernetSettings"></a>

#### Declaration

```text
[JsonProperty("ethParams")]
public EthernetSettingsV1 EthernetSettings { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [EthernetSettingsV1](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EthernetSettingsV1.html) |  |

### Id <a id="FBoxClientDriver_Contract_PlcDevice_Id"></a>

设备ID （不唯一）

#### Declaration

```text
public int Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Manufacturer <a id="FBoxClientDriver_Contract_PlcDevice_Manufacturer"></a>

厂家

#### Declaration

```text
[JsonProperty("mfr")]
public string Manufacturer { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### MaxStationNo <a id="FBoxClientDriver_Contract_PlcDevice_MaxStationNo"></a>

最大站号

#### Declaration

```text
public int MaxStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MiniDrivers <a id="FBoxClientDriver_Contract_PlcDevice_MiniDrivers"></a>

mini驱动

#### Declaration

```text
public IList MiniDrivers { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[MiniDeviceDriverInfo](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.MiniDeviceDriverInfo.html)&gt; |  |

### MinStationNo <a id="FBoxClientDriver_Contract_PlcDevice_MinStationNo"></a>

最小站号

#### Declaration

```text
public int MinStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Name <a id="FBoxClientDriver_Contract_PlcDevice_Name"></a>

设备名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Registers <a id="FBoxClientDriver_Contract_PlcDevice_Registers"></a>

寄存器列表

#### Declaration

```text
[JsonProperty("regs")]
public IList Registers { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[RegisterInfo](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RegisterInfo.html)&gt; |  |

### SerialPortSettings <a id="FBoxClientDriver_Contract_PlcDevice_SerialPortSettings"></a>

串口通讯默认参数

#### Declaration

```text
[JsonProperty("comPortParams")]
public SerialPortSettingsV1 SerialPortSettings { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [SerialPortSettingsV1](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.SerialPortSettingsV1.html) |  |

### SupportedPlcs <a id="FBoxClientDriver_Contract_PlcDevice_SupportedPlcs"></a>

支持的PLC类型

#### Declaration

```text
public IList SupportedPlcs { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.String&gt; |  |

