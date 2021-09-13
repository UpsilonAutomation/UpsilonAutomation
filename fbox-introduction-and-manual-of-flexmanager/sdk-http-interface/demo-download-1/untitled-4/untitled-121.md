# HistoryDataV2

历史记录（原始）

#### Inheritance

System.Object

HistoryDataV2

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

#### Syntax <a id="FBoxClientDriver_Contract_HistoryDataV2_syntax"></a>

```text
public class HistoryDataV2
```

## Properties <a id="properties"></a>

### HdataDefId <a id="FBoxClientDriver_Contract_HistoryDataV2_HdataDefId"></a>

#### Declaration

```text
[JsonProperty("i")]
public long HdataDefId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Time <a id="FBoxClientDriver_Contract_HistoryDataV2_Time"></a>

时间

#### Declaration

```text
public DateTime Time { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### TimeJsEpoch <a id="FBoxClientDriver_Contract_HistoryDataV2_TimeJsEpoch"></a>

时间 \(UTC 从1970.1.1开始\)

#### Declaration

```text
[JsonProperty("t")]
public long TimeJsEpoch { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Value <a id="FBoxClientDriver_Contract_HistoryDataV2_Value"></a>

值

#### Declaration

```text
[JsonProperty("v")]
public object Value { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Object |  |

