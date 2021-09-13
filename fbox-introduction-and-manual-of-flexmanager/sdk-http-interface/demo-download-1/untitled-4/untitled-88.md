# HDataControl

使能控制\(注意：使能控制 数据类型只能支持位类型\)

#### Inheritance

System.Object

HDataControl

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

#### Syntax <a id="FBoxClientDriver_Contract_HDataControl_syntax"></a>

```text
public class HDataControl
```

## Properties <a id="properties"></a>

### DataType <a id="FBoxClientDriver_Contract_HDataControl_DataType"></a>

数据类型 【对用到客户端选择的数据类型 DataType枚举】

#### Declaration

```text
public DataType DataType { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### DeviceId <a id="FBoxClientDriver_Contract_HDataControl_DeviceId"></a>

设备ID 【选择设备：BoxDeviceInfo中获取赋值】

#### Declaration

```text
public int DeviceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MainAddress <a id="FBoxClientDriver_Contract_HDataControl_MainAddress"></a>

主地址 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-MainAddressType】,8进制 16进制都转换成10进制传入参数,跟PLC有关

#### Declaration

```text
public int MainAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Port <a id="FBoxClientDriver_Contract_HDataControl_Port"></a>

串口1：0，串口2：1，串口3：2，以太网：4096以上 【选择设备：BoxDeviceInfo中获取赋值】

#### Declaration

```text
public int Port { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegId <a id="FBoxClientDriver_Contract_HDataControl_RegId"></a>

寄存器ID 【对应到客户端选择地址类型 DeviceSpecification-RegisterInfo-Id】

#### Declaration

```text
public int RegId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegWidth <a id="FBoxClientDriver_Contract_HDataControl_RegWidth"></a>

地址宽度 【对应到客户端选择地址类型 DeviceSpecification-RegisterInfo-IoWidth】

#### Declaration

```text
public DataWidth RegWidth { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |  |

### ServiceId <a id="FBoxClientDriver_Contract_HDataControl_ServiceId"></a>

服务ID

#### Declaration

```text
public int ServiceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StationNo <a id="FBoxClientDriver_Contract_HDataControl_StationNo"></a>

站号 【输入框输入】

#### Declaration

```text
public int StationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Statue <a id="FBoxClientDriver_Contract_HDataControl_Statue"></a>

使能状态

#### Declaration

```text
public bool Statue { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### SubAddress <a id="FBoxClientDriver_Contract_HDataControl_SubAddress"></a>

子地址 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-SubAddressType】,8进制 16进制都转换成10进制传入参数,跟PLC有关

#### Declaration

```text
public int SubAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubIndex <a id="FBoxClientDriver_Contract_HDataControl_SubIndex"></a>

子地址索引 【对应到客户端主地址：主地址填写类型 DeviceSpecification-RegisterInfo-SubIndexType】,8进制 16进制都转换成10进制传入参数,跟PLC有关

#### Declaration

```text
public int SubIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

