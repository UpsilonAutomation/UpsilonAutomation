# ByRowHistoryDataRow

#### Inheritance

System.Object

ByRowHistoryDataRow

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

#### Syntax <a id="FBoxClientDriver_Contract_Entity_ByRowHistoryDataRow_syntax"></a>

```text
public class ByRowHistoryDataRow
```

## Properties <a id="properties"></a>

### Time <a id="FBoxClientDriver_Contract_Entity_ByRowHistoryDataRow_Time"></a>

Unix timestamp utc 时间，注意

#### Declaration

```text
[JsonProperty("t")]
[JsonConverter(typeof(JavascriptEpochConverter))]
public DateTime Time { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### Values <a id="FBoxClientDriver_Contract_Entity_ByRowHistoryDataRow_Values"></a>

#### Declaration

```text
[JsonProperty("c")]
public IList
```

