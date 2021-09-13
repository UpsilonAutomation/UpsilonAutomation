# AddOrUpdatePlcDeviceV2

PLC驱动设备V2

#### Inheritance

System.Object

AddOrUpdatePlcDeviceV2

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

#### Syntax <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_syntax"></a>

```text
public class AddOrUpdatePlcDeviceV2
```

## Properties <a id="properties"></a>

### Alias <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_Alias"></a>

别名

#### Declaration

```text
public string Alias { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BaudRate <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_BaudRate"></a>

波特率

#### Declaration

```text
public int BaudRate { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### BroadcastStationNo <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_BroadcastStationNo"></a>

广播站号

#### Declaration

```text
public int BroadcastStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Class <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_Class"></a>

设备类型

#### Declaration

```text
public PlcClass Class { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PlcClass](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcClass.html) |  |

### DataBits <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_DataBits"></a>

数据位

#### Declaration

```text
public int DataBits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DefaultStationNo <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_DefaultStationNo"></a>

默认站号

#### Declaration

```text
public int DefaultStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### EnableBroadcast <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_EnableBroadcast"></a>

是否启用广播站号

#### Declaration

```text
public bool EnableBroadcast { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Interface <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_Interface"></a>

#### Declaration

```text
public DeviceInterfaceTypes Interface { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DeviceInterfaceTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DeviceInterfaceTypes.html) |  |

### Ip <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_Ip"></a>

网络设备IP地址

#### Declaration

```text
public string Ip { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### ParityType <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_ParityType"></a>

校验位

#### Declaration

```text
public ParityType ParityType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [ParityType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ParityType.html) |  |

### PlcAdvancedSettings <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_PlcAdvancedSettings"></a>

#### Declaration

```text
[JsonProperty("advanced")]
public PlcAdvancedSettings PlcAdvancedSettings { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PlcAdvancedSettings](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcAdvancedSettings.html) |  |

### PlcId <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_PlcId"></a>

PLC Id（不唯一）

#### Declaration

```text
public int PlcId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### PlcName <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_PlcName"></a>

PLC名称

#### Declaration

```text
public string PlcName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Port <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_Port"></a>

网络设备端口号

#### Declaration

```text
public int Port { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### PortNo <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_PortNo"></a>

编号

#### Declaration

```text
public int PortNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SlaveNo <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_SlaveNo"></a>

从设备号

#### Declaration

```text
public int SlaveNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StopBits <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_StopBits"></a>

停止位

#### Declaration

```text
public int StopBits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Type <a id="FBoxClientDriver_Contract_AddOrUpdatePlcDeviceV2_Type"></a>

#### Declaration

```text
public ServerType Type { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [ServerType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ServerType.html) |  |

