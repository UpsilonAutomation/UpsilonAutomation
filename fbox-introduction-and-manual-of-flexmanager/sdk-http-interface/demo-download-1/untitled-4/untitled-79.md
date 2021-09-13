# GetHistoryDataArgs

#### Inheritance

System.Object

GetHistoryDataArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_GetHistoryDataArgs_syntax"></a>

```text
public class GetHistoryDataArgs
```

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_GetHistoryDataArgs_BoxNo"></a>

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### EndTime <a id="FBoxClientDriver_Contract_GetHistoryDataArgs_EndTime"></a>

#### Declaration

```text
public DateTime EndTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### HdataChannelNames <a id="FBoxClientDriver_Contract_GetHistoryDataArgs_HdataChannelNames"></a>

#### Declaration

```text
[JsonProperty("cnames")]
public IList HdataChannelNames { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.String&gt; |  |

### HdataItemName <a id="FBoxClientDriver_Contract_GetHistoryDataArgs_HdataItemName"></a>

#### Declaration

```text
[JsonProperty("name")]
public string HdataItemName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Limit <a id="FBoxClientDriver_Contract_GetHistoryDataArgs_Limit"></a>

#### Declaration

```text
public int Limit { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StartTime <a id="FBoxClientDriver_Contract_GetHistoryDataArgs_StartTime"></a>

#### Declaration

```text
public DateTime StartTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### TimeRange <a id="FBoxClientDriver_Contract_GetHistoryDataArgs_TimeRange"></a>

#### Declaration

```text
[JsonProperty("tr")]
public TimeRangeTypes TimeRange { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [TimeRangeTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.TimeRangeTypes.html) |  |

