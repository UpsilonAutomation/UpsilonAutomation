# GetSomeHdataItemArgs

#### Inheritance

System.Object

GetSomeHdataItemArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_GetSomeHdataItemArgs_syntax"></a>

```text
public class GetSomeHdataItemArgs
```

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_GetSomeHdataItemArgs_BoxNo"></a>

盒子号码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Ids <a id="FBoxClientDriver_Contract_GetSomeHdataItemArgs_Ids"></a>

条目Id集合,与Names选择其中一个

#### Declaration

```text
public IList Ids { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; |  |

### Names <a id="FBoxClientDriver_Contract_GetSomeHdataItemArgs_Names"></a>

条目名称集合,与Ids选择其中一个

#### Declaration

```text
public IList Names { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.String&gt; |  |

