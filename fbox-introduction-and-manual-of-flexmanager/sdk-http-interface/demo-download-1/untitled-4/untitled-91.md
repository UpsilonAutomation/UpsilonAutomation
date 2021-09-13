# HdataDtoV2

历史记录条目基类

#### Inheritance

System.Object

HdataDtoV2

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

#### Syntax <a id="FBoxClientDriver_Contract_HdataDtoV2_syntax"></a>

```text
public class HdataDtoV2 : DataSourceDtoV2
```

## Properties <a id="properties"></a>

### ControlOptions <a id="FBoxClientDriver_Contract_HdataDtoV2_ControlOptions"></a>

#### Declaration

```text
[JsonProperty("ctrlOptions")]
public HDataControlOptionsV2 ControlOptions { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) |  |

### FractionalDigits <a id="FBoxClientDriver_Contract_HdataDtoV2_FractionalDigits"></a>

小数位

#### Declaration

```text
[JsonProperty("fracDigits")]
public int FractionalDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IntegralDigits <a id="FBoxClientDriver_Contract_HdataDtoV2_IntegralDigits"></a>

整数位

#### Declaration

```text
[JsonProperty("intDigits")]
public int IntegralDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IsControl <a id="FBoxClientDriver_Contract_HdataDtoV2_IsControl"></a>

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

### Memo <a id="FBoxClientDriver_Contract_HdataDtoV2_Memo"></a>

备注

#### Declaration

```text
[JsonProperty("memo")]
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_HdataDtoV2_Name"></a>

名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### RecordingPeriod <a id="FBoxClientDriver_Contract_HdataDtoV2_RecordingPeriod"></a>

采样时间（单位：s）

#### Declaration

```text
[JsonProperty("samplePeriod")]
public int RecordingPeriod { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

