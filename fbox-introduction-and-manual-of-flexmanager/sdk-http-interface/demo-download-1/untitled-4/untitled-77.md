# GetDMonValueArgs

获取监控点数据接口

#### Inheritance

System.Object

System.EventArgs

GetDMonValueArgs

#### Inherited Members

System.EventArgs.Empty

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver.Contract**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_GetDMonValueArgs_syntax"></a>

```text
public class GetDMonValueArgs : EventArgs
```

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_GetDMonValueArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Ids <a id="FBoxClientDriver_Contract_GetDMonValueArgs_Ids"></a>

#### Declaration

```text
public IList Ids { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; |  |

### Names <a id="FBoxClientDriver_Contract_GetDMonValueArgs_Names"></a>

#### Declaration

```text
public IList Names { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.String&gt; |  |

### NamesWithGroup <a id="FBoxClientDriver_Contract_GetDMonValueArgs_NamesWithGroup"></a>

\(监控点名称,监控点组名称）集合，与[Names]()二选一，用于不同组下有同名监控点的情况

#### Declaration

```text
public IList> NamesWithGroup { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.Tuple&lt;System.String, System.String&gt;&gt; |  |

### Timeout <a id="FBoxClientDriver_Contract_GetDMonValueArgs_Timeout"></a>

最大读取超时，null为取服务器默认值

#### Declaration

```text
public int? Timeout { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Nullable&lt;System.Int32&gt; |  |

### UseCache <a id="FBoxClientDriver_Contract_GetDMonValueArgs_UseCache"></a>

是否使用服务器缓存数据

#### Declaration

```text
public bool UseCache { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

