# BoxDto

#### Inheritance

System.Object

BoxDto

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

#### Syntax <a id="FBoxClientDriver_Contract_Entity_BoxDto_syntax"></a>

## Constructors <a id="constructors"></a>

### BoxDto\(\) <a id="FBoxClientDriver_Contract_Entity_BoxDto__ctor"></a>

#### Declaration

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_Entity_BoxDto_BoxNo"></a>

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxType <a id="FBoxClientDriver_Contract_Entity_BoxDto_BoxType"></a>

#### Declaration

```text
public BoxTypes BoxType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxTypes.html) |  |

### CommServer <a id="FBoxClientDriver_Contract_Entity_BoxDto_CommServer"></a>

#### Declaration

```text
[JsonProperty("cs")]
public CommServer CommServer { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [CommServer](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.CommServer.html) |  |

### ConnectionState <a id="FBoxClientDriver_Contract_Entity_BoxDto_ConnectionState"></a>

#### Declaration

```text
public BoxConnectionState ConnectionState { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) |  |

### Disabled <a id="FBoxClientDriver_Contract_Entity_BoxDto_Disabled"></a>

#### Declaration

```text
[JsonProperty("disabled")]
public bool Disabled { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Id <a id="FBoxClientDriver_Contract_Entity_BoxDto_Id"></a>

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Memo <a id="FBoxClientDriver_Contract_Entity_BoxDto_Memo"></a>

#### Declaration

```text
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### NetworkType <a id="FBoxClientDriver_Contract_Entity_BoxDto_NetworkType"></a>

#### Declaration

```text
[JsonProperty("net")]
public NetworkTypes NetworkType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [NetworkTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.NetworkTypes.html) |  |

