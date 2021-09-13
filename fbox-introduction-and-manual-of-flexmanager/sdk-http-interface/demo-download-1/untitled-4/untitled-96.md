# GetDeviceSpecificationArgs

获取设备规格参数

#### Inheritance

System.Object

GetDeviceSpecificationArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_GetDeviceSpecificationArgs_syntax"></a>

```text
public class GetDeviceSpecificationArgs
```

## Constructors <a id="constructors"></a>

### GetDeviceSpecificationArgs\(\) <a id="FBoxClientDriver_Contract_GetDeviceSpecificationArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public GetDeviceSpecificationArgs()
```

### GetDeviceSpecificationArgs\(Int32, DataType\) <a id="FBoxClientDriver_Contract_GetDeviceSpecificationArgs__ctor_System_Int32_FBoxClientDriver_Contract_DataType_"></a>

构造函数

#### Declaration

```text
public GetDeviceSpecificationArgs(int deviceId, DataType dataType)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int32 | deviceId | 设备ID |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 |

## Properties <a id="properties"></a>

### DataType <a id="FBoxClientDriver_Contract_GetDeviceSpecificationArgs_DataType"></a>

数据类型

#### Declaration

```text
public DataType DataType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### DeviceId <a id="FBoxClientDriver_Contract_GetDeviceSpecificationArgs_DeviceId"></a>

设备ID

#### Declaration

```text
public int DeviceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

