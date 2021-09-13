# DeviceSpecification

设备规格信息

#### Inheritance

System.Object

DeviceSpecification

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

#### Syntax <a id="FBoxClientDriver_Contract_DeviceSpecification_syntax"></a>

```text
public class DeviceSpecification
```

## Properties <a id="properties"></a>

### DefaultStationNo <a id="FBoxClientDriver_Contract_DeviceSpecification_DefaultStationNo"></a>

默认站号

#### Declaration

```text
public int DefaultStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Id <a id="FBoxClientDriver_Contract_DeviceSpecification_Id"></a>

设备ID

#### Declaration

```text
public int Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MaxStationNo <a id="FBoxClientDriver_Contract_DeviceSpecification_MaxStationNo"></a>

最大站号

#### Declaration

```text
public int MaxStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MinStationNo <a id="FBoxClientDriver_Contract_DeviceSpecification_MinStationNo"></a>

最小站号

#### Declaration

```text
public int MinStationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Name <a id="FBoxClientDriver_Contract_DeviceSpecification_Name"></a>

设备名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Registers <a id="FBoxClientDriver_Contract_DeviceSpecification_Registers"></a>

寄存器信息

#### Declaration

```text
public IList Registers { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[RegisterInfo](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RegisterInfo.html)&gt; |  |

### SerialPortSettings <a id="FBoxClientDriver_Contract_DeviceSpecification_SerialPortSettings"></a>

串口通讯默认参数

#### Declaration

```text
public SerialPortSettings SerialPortSettings { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [SerialPortSettings](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.SerialPortSettings.html) |  |

## Methods <a id="methods"></a>

### FilterRegisters\(DataType\) <a id="FBoxClientDriver_Contract_DeviceSpecification_FilterRegisters_FBoxClientDriver_Contract_DataType_"></a>

通过数据类型过滤寄存器列表

#### Declaration

```text
public IList FilterRegisters(DataType dataType)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[RegisterInfo](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RegisterInfo.html)&gt; |  |

