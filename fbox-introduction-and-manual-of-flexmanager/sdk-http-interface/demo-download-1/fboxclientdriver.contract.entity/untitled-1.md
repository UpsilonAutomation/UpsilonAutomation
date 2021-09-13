# HdataItem

#### Inheritance

System.Object

HdataItem

#### Inherited Members

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver.Contract.Entity**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_Entity_HdataItem_syntax"></a>

## Properties <a id="properties"></a>

### BoxId <a id="FBoxClientDriver_Contract_Entity_HdataItem_BoxId"></a>

盒子Id

#### Declaration

```text
public long BoxId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Channels <a id="FBoxClientDriver_Contract_Entity_HdataItem_Channels"></a>

通道集合

#### Declaration

```text
public IList Channels { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[HdataChannel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.HdataChannel.html)&gt; |  |

### ControlOptions <a id="FBoxClientDriver_Contract_Entity_HdataItem_ControlOptions"></a>

#### Declaration

```text
[JsonProperty("ctrl")]
public HDataControlOptionsV2 ControlOptions { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) |  |

### IsControl <a id="FBoxClientDriver_Contract_Entity_HdataItem_IsControl"></a>

是否使能设置

#### Declaration

```text
[JsonProperty("hasCtrl")]
public bool IsControl { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Name <a id="FBoxClientDriver_Contract_Entity_HdataItem_Name"></a>

名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### RecordingPeriod <a id="FBoxClientDriver_Contract_Entity_HdataItem_RecordingPeriod"></a>

采集周期

#### Declaration

```text
[JsonProperty("period")]
public int RecordingPeriod { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Uid <a id="FBoxClientDriver_Contract_Entity_HdataItem_Uid"></a>

主键

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

