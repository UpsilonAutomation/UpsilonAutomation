# BoxDeviceInfo

盒子上的某个设备的描述类

#### Inheritance

System.Object

BoxDeviceInfo

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

#### Syntax <a id="FBoxClientDriver_Contract_BoxDeviceInfo_syntax"></a>

```text
public class BoxDeviceInfo
```

## Properties <a id="properties"></a>

### DeviceId <a id="FBoxClientDriver_Contract_BoxDeviceInfo_DeviceId"></a>

设备ID

#### Declaration

```text
public int DeviceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DeviceName <a id="FBoxClientDriver_Contract_BoxDeviceInfo_DeviceName"></a>

设备名称

#### Declaration

```text
public string DeviceName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### IP <a id="FBoxClientDriver_Contract_BoxDeviceInfo_IP"></a>

以太网设备静态IP地址

#### Declaration

```text
public string IP { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Port <a id="FBoxClientDriver_Contract_BoxDeviceInfo_Port"></a>

以太网设备监听端口

#### Declaration

```text
public int Port { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### PortNo <a id="FBoxClientDriver_Contract_BoxDeviceInfo_PortNo"></a>

当设备接口为串口时，表示串口号，从0开始。

#### Declaration

```text
public int PortNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ServerId <a id="FBoxClientDriver_Contract_BoxDeviceInfo_ServerId"></a>

设备类型，0表示串口设备，2表示以太网设备

#### Declaration

```text
public int ServerId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StationNo <a id="FBoxClientDriver_Contract_BoxDeviceInfo_StationNo"></a>

站号

#### Declaration

```text
public int StationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

