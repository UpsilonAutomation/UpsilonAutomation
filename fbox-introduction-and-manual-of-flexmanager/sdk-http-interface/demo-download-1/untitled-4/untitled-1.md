# BitStateLabel

位类型数据标签

#### Inheritance

System.Object

BitStateLabel

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

#### Syntax <a id="FBoxClientDriver_Contract_BitStateLabel_syntax"></a>

```text
public class BitStateLabel
```

## Properties <a id="properties"></a>

### FalseLabel <a id="FBoxClientDriver_Contract_BitStateLabel_FalseLabel"></a>

值为false时的文本

#### Declaration

```text
[JsonProperty("ftext")]
public string FalseLabel { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### TrueLabel <a id="FBoxClientDriver_Contract_BitStateLabel_TrueLabel"></a>

值为True时的文本

#### Declaration

```text
[JsonProperty("ttext")]
public string TrueLabel { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

