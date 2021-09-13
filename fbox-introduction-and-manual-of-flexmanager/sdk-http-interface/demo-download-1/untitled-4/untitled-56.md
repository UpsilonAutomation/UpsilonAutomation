# DataMonitorGroup

检测点组别

#### Inheritance

System.Object

DataMonitorGroup

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

#### Syntax <a id="FBoxClientDriver_Contract_DataMonitorGroup_syntax"></a>

```text
public class DataMonitorGroup
```

## Properties <a id="properties"></a>

### DataMonitorDefinitions <a id="FBoxClientDriver_Contract_DataMonitorGroup_DataMonitorDefinitions"></a>

检测点组下的监测点条目

#### Declaration

```text
public IList DataMonitorDefinitions { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[DataMonitorDefinition](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorDefinition.html)&gt; |  |

### GroupName <a id="FBoxClientDriver_Contract_DataMonitorGroup_GroupName"></a>

监测点组的名称

#### Declaration

```text
public string GroupName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_DataMonitorGroup_Uid"></a>

监测点组的UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

