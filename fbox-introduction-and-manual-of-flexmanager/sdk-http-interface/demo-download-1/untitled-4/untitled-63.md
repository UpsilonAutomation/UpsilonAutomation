# DataMonitorValueChangedArgs

监测点数据通知参数

#### Inheritance

System.Object

System.EventArgs

DataMonitorValueChangedArgs

#### Inherited Members

System.EventArgs.Empty

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver.Contract**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_DataMonitorValueChangedArgs_syntax"></a>

```text
public class DataMonitorValueChangedArgs : EventArgs
```

## Properties <a id="properties"></a>

### BoxId <a id="FBoxClientDriver_Contract_DataMonitorValueChangedArgs_BoxId"></a>

盒子ID

#### Declaration

```text
public long BoxId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### BoxNo <a id="FBoxClientDriver_Contract_DataMonitorValueChangedArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### GroupName <a id="FBoxClientDriver_Contract_DataMonitorValueChangedArgs_GroupName"></a>

组名（根据服务器配置，可能为空）

#### Declaration

```text
public string GroupName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_DataMonitorValueChangedArgs_Name"></a>

监控点名称（根据服务器配置，可能为空）

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Status <a id="FBoxClientDriver_Contract_DataMonitorValueChangedArgs_Status"></a>

条目状态

#### Declaration

```text
public DMonStatus Status { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DMonStatus](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DMonStatus.html) |  |

### Uid <a id="FBoxClientDriver_Contract_DataMonitorValueChangedArgs_Uid"></a>

检测点条目的UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Value <a id="FBoxClientDriver_Contract_DataMonitorValueChangedArgs_Value"></a>

检测点条目的值

#### Declaration

```text
public object Value { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Object |  |

