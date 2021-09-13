# HdataItemDto

#### Inheritance

System.Object

HdataItemDto

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

#### Syntax <a id="FBoxClientDriver_Contract_HdataItemDto_syntax"></a>

```text
public class HdataItemDto
```

## Properties <a id="properties"></a>

### ControlOptions <a id="FBoxClientDriver_Contract_HdataItemDto_ControlOptions"></a>

使能控制

#### Declaration

```text
[JsonProperty("ctrl")]
public HDataControlOptionsV2 ControlOptions { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) |  |

### IsControl <a id="FBoxClientDriver_Contract_HdataItemDto_IsControl"></a>

是否使能控制

#### Declaration

```text
[JsonProperty("hasCtrl")]
public bool IsControl { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Name <a id="FBoxClientDriver_Contract_HdataItemDto_Name"></a>

名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### RecordingPeriod <a id="FBoxClientDriver_Contract_HdataItemDto_RecordingPeriod"></a>

采样周期

#### Declaration

```text
[JsonProperty("period")]
public int RecordingPeriod { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

