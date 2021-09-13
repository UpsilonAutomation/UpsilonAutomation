# ExportHistoryDataCsvArgs

导出历史记录参数

#### Inheritance

System.Object

ExportHistoryDataCsvArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_ExportHistoryDataCsvArgs_syntax"></a>

```text
public class ExportHistoryDataCsvArgs
```

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_ExportHistoryDataCsvArgs_BoxNo"></a>

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### EndTime <a id="FBoxClientDriver_Contract_ExportHistoryDataCsvArgs_EndTime"></a>

#### Declaration

```text
public DateTime EndTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### HdataChannelNames <a id="FBoxClientDriver_Contract_ExportHistoryDataCsvArgs_HdataChannelNames"></a>

#### Declaration

```text
[JsonProperty("cnames")]
public IList HdataChannelNames { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.String&gt; |  |

### HdataItemName <a id="FBoxClientDriver_Contract_ExportHistoryDataCsvArgs_HdataItemName"></a>

#### Declaration

```text
[JsonProperty("name")]
public string HdataItemName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### StartTime <a id="FBoxClientDriver_Contract_ExportHistoryDataCsvArgs_StartTime"></a>

#### Declaration

```text
public DateTime StartTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### TimeRange <a id="FBoxClientDriver_Contract_ExportHistoryDataCsvArgs_TimeRange"></a>

#### Declaration

```text
[JsonProperty("tr")]
public TimeRangeTypes TimeRange { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [TimeRangeTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.TimeRangeTypes.html) |  |

