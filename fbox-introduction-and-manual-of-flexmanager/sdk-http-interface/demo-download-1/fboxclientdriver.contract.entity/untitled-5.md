# FBox

#### Inheritance

System.Object

FBox

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

#### Syntax <a id="FBoxClientDriver_Contract_Entity_FBox_syntax"></a>

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_Entity_FBox_BoxNo"></a>

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxType <a id="FBoxClientDriver_Contract_Entity_FBox_BoxType"></a>

#### Declaration

```text
public BoxTypes BoxType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxTypes.html) |  |

### CommServer <a id="FBoxClientDriver_Contract_Entity_FBox_CommServer"></a>

#### Declaration

```text
[JsonProperty("cs")]
public CommServer CommServer { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [CommServer](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.CommServer.html) |  |

### ConnectionState <a id="FBoxClientDriver_Contract_Entity_FBox_ConnectionState"></a>

#### Declaration

```text
public BoxConnectionState ConnectionState { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) |  |

### CurrentSessionId <a id="FBoxClientDriver_Contract_Entity_FBox_CurrentSessionId"></a>

#### Declaration

```text
public int CurrentSessionId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Id <a id="FBoxClientDriver_Contract_Entity_FBox_Id"></a>

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### UserPassword <a id="FBoxClientDriver_Contract_Entity_FBox_UserPassword"></a>

#### Declaration

```text
public string UserPassword { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

