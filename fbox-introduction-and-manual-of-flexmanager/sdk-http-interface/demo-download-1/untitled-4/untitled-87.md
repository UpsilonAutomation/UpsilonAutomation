# HdataChannelDto

#### Inheritance

System.Object

HdataChannelDto

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

#### Syntax <a id="FBoxClientDriver_Contract_HdataChannelDto_syntax"></a>

```text
public class HdataChannelDto : DataSourceDtoV2
```

## Properties <a id="properties"></a>

### ChannelName <a id="FBoxClientDriver_Contract_HdataChannelDto_ChannelName"></a>

#### Declaration

```text
[JsonProperty("name")]
public string ChannelName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Description <a id="FBoxClientDriver_Contract_HdataChannelDto_Description"></a>

#### Declaration

```text
[JsonProperty("desc")]
public string Description { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### FractionalDigits <a id="FBoxClientDriver_Contract_HdataChannelDto_FractionalDigits"></a>

#### Declaration

```text
[JsonProperty("fracDigits")]
public int FractionalDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IntegralDigits <a id="FBoxClientDriver_Contract_HdataChannelDto_IntegralDigits"></a>

#### Declaration

```text
[JsonProperty("intDigits")]
public int IntegralDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Unit <a id="FBoxClientDriver_Contract_HdataChannelDto_Unit"></a>

#### Declaration

```text
public string Unit { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

