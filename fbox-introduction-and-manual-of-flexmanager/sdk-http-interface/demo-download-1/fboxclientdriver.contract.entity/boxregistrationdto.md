# BoxRegistrationDto

#### Inheritance

System.Object

BoxRegistrationDto

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

#### Syntax <a id="FBoxClientDriver_Contract_Entity_BoxRegistrationDto_syntax"></a>

```text
public class BoxRegistrationDto
```

## Constructors <a id="constructors"></a>

### BoxRegistrationDto\(\) <a id="FBoxClientDriver_Contract_Entity_BoxRegistrationDto__ctor"></a>

#### Declaration

```text
public BoxRegistrationDto()
```

## Properties <a id="properties"></a>

### Alias <a id="FBoxClientDriver_Contract_Entity_BoxRegistrationDto_Alias"></a>

#### Declaration

```text
public string Alias { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Box <a id="FBoxClientDriver_Contract_Entity_BoxRegistrationDto_Box"></a>

#### Declaration

```text
public BoxDto Box { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxDto](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.BoxDto.html) |  |

### BoxId <a id="FBoxClientDriver_Contract_Entity_BoxRegistrationDto_BoxId"></a>

#### Declaration

```text
[JsonProperty("boxUid")]
public long BoxId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Id <a id="FBoxClientDriver_Contract_Entity_BoxRegistrationDto_Id"></a>

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Owned <a id="FBoxClientDriver_Contract_Entity_BoxRegistrationDto_Owned"></a>

#### Declaration

```text
[JsonProperty("owned")]
public bool Owned { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

