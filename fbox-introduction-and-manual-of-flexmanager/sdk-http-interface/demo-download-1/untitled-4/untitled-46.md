# BoxStateChangedEvent

#### Inheritance

System.Object

BoxStateChangedEvent

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

#### Syntax <a id="FBoxClientDriver_Contract_BoxStateChangedEvent_syntax"></a>

```text
public class BoxStateChangedEvent
```

## Properties <a id="properties"></a>

### BoxId <a id="FBoxClientDriver_Contract_BoxStateChangedEvent_BoxId"></a>

#### Declaration

```text
public long BoxId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### BoxNo <a id="FBoxClientDriver_Contract_BoxStateChangedEvent_BoxNo"></a>

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### State <a id="FBoxClientDriver_Contract_BoxStateChangedEvent_State"></a>

#### Declaration

```text
public BoxConnectionState State { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) |  |

### Timestamp <a id="FBoxClientDriver_Contract_BoxStateChangedEvent_Timestamp"></a>

#### Declaration

```text
public DateTime Timestamp { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

