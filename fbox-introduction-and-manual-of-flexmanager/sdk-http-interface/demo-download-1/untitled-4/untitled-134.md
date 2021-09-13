# PlcDeviceDtoV2

获取设备规格参数

#### Inheritance

System.Object

PlcDeviceDtoV2

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

#### Syntax <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_syntax"></a>

```text
public class PlcDeviceDtoV2
```

## Constructors <a id="constructors"></a>

### PlcDeviceDtoV2\(\) <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2__ctor"></a>

无参构造函数

#### Declaration

### PlcDeviceDtoV2\(Int32, String, String, ServerType, PlcAdvancedSettings, Int32, PlcDongFlag, DeviceInterfaceTypes, Int32, Int32, Int32, ParityType, PlcClass, String, Int32, Boolean, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2__ctor_System_Int32_System_String_System_String_FBoxClientDriver_Contract_ServerType_FBoxClientDriver_Contract_PlcAdvancedSettings_System_Int32_FBoxClientDriver_Contract_PlcDongFlag_FBoxClientDriver_Contract_DeviceInterfaceTypes_System_Int32_System_Int32_System_Int32_FBoxClientDriver_Contract_ParityType_FBoxClientDriver_Contract_PlcClass_System_String_System_Int32_System_Boolean_System_Int32_System_Int32_System_Int32_"></a>

#### Declaration

```text
public PlcDeviceDtoV2(int plcId, string plcName, string alias, ServerType type, PlcAdvancedSettings plcAdvancedSettings, int portNo, PlcDongFlag plcDongleFlag, DeviceInterfaceTypes interface, int baudRate, int dataBits, int stopBits, ParityType parityType, PlcClass class, string ip, int port, bool enableBroadcast, int broadcastStationNo, int defaultStationNo, int slaveNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int32 | plcId | plcId |
| System.String | plcName | Plc名称 |
| System.String | alias | Plc别名 |
| [ServerType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ServerType.html) | type | 驱动类型[ServerType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ServerType.html) |
| [PlcAdvancedSettings](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcAdvancedSettings.html) | plcAdvancedSettings | 高级设置[PlcAdvancedSettings]() |
| System.Int32 | portNo | 站号 |
| [PlcDongFlag](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcDongFlag.html) | plcDongleFlag | 远程停机状态[PlcDongFlag](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcDongFlag.html) |
| [DeviceInterfaceTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DeviceInterfaceTypes.html) | interface | 通讯类型[DeviceInterfaceTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DeviceInterfaceTypes.html) |
| System.Int32 | baudRate | 波特率 |
| System.Int32 | dataBits | 数据位 |
| System.Int32 | stopBits | 停止位 |
| [ParityType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ParityType.html) | parityType | 校验位[ParityType]() |
| [PlcClass](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcClass.html) | class | 主从设备[PlcClass](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcClass.html) |
| System.String | ip | Ip地址 |
| System.Int32 | port | 以太网端口号 |
| System.Boolean | enableBroadcast | 使能广播站号 |
| System.Int32 | broadcastStationNo | 广播站号 |
| System.Int32 | defaultStationNo | 默认站号 |
| System.Int32 | slaveNo | 从设备号 |

## Properties <a id="properties"></a>

### Alias <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_Alias"></a>

PLC别名

#### Declaration

```text
public string Alias { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BaudRate <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_BaudRate"></a>

波特率

#### Declaration

```text
public int BaudRate { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### BroadcastStationNo <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_BroadcastStationNo"></a>

广播站号

#### Declaration

```text
public int BroadcastStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Class <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_Class"></a>

PLC为主或从设备

#### Declaration

```text
public PlcClass Class { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PlcClass](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcClass.html) |  |

### DataBits <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_DataBits"></a>

数据位

#### Declaration

```text
public int DataBits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DefaultStationNo <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_DefaultStationNo"></a>

默认广播站号

#### Declaration

```text
public int DefaultStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### EnableBroadcast <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_EnableBroadcast"></a>

使能广播站号

#### Declaration

```text
public bool EnableBroadcast { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Interface <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_Interface"></a>

通讯类型

#### Declaration

```text
public DeviceInterfaceTypes Interface { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DeviceInterfaceTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DeviceInterfaceTypes.html) |  |

### Ip <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_Ip"></a>

Ip地址

#### Declaration

```text
public string Ip { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### ParityType <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_ParityType"></a>

校验位

#### Declaration

```text
public ParityType ParityType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [ParityType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ParityType.html) |  |

### PlcAdvancedSettings <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_PlcAdvancedSettings"></a>

高级设置

#### Declaration

```text
[JsonProperty("advanced")]
public PlcAdvancedSettings PlcAdvancedSettings { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PlcAdvancedSettings](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcAdvancedSettings.html) |  |

### PlcDongleFlag <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_PlcDongleFlag"></a>

远程停机状态、盒子在线状态

#### Declaration

```text
public PlcDongFlag PlcDongleFlag { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PlcDongFlag](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcDongFlag.html) |  |

### PlcId <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_PlcId"></a>

PlcId

#### Declaration

```text
public int PlcId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### PlcName <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_PlcName"></a>

PLC名称

#### Declaration

```text
public string PlcName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Port <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_Port"></a>

以太网端口号

#### Declaration

```text
public int Port { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### PortNo <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_PortNo"></a>

站号

#### Declaration

```text
public int PortNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SlaveNo <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_SlaveNo"></a>

从设备号

#### Declaration

```text
public int SlaveNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StopBits <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_StopBits"></a>

停止位

#### Declaration

```text
public int StopBits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Type <a id="FBoxClientDriver_Contract_PlcDeviceDtoV2_Type"></a>

PLC类型，串口或者以太网

#### Declaration

```text
public ServerType Type { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [ServerType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ServerType.html) |  |

