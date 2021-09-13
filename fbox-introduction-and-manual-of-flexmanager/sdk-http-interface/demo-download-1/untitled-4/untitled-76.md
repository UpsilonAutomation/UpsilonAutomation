# DmonItemDtoV2

监控点条目属性

#### Inheritance

System.Object

DmonItemDtoV2

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

#### Syntax <a id="FBoxClientDriver_Contract_DmonItemDtoV2_syntax"></a>

```text
public class DmonItemDtoV2 : DMonDtoV2
```

## Properties <a id="properties"></a>

### Id <a id="FBoxClientDriver_Contract_DmonItemDtoV2_Id"></a>

监控点Id

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### IsDeviceChanged <a id="FBoxClientDriver_Contract_DmonItemDtoV2_IsDeviceChanged"></a>

设备是否移除

#### Declaration

```text
[JsonProperty("deviceChanged")]
public bool IsDeviceChanged { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### TaskState <a id="FBoxClientDriver_Contract_DmonItemDtoV2_TaskState"></a>

#### Declaration

```text
[JsonProperty("tstate")]
public TaskState TaskState { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [TaskState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.TaskState.html) |  |

