# BoxRegistration

#### Inheritance

System.Object

BoxRegistration

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

#### Syntax <a id="FBoxClientDriver_Contract_Entity_BoxRegistration_syntax"></a>

```text
public class BoxRegistration
```

## Properties <a id="properties"></a>

### Alias <a id="FBoxClientDriver_Contract_Entity_BoxRegistration_Alias"></a>

#### Declaration

```text
public string Alias { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Box <a id="FBoxClientDriver_Contract_Entity_BoxRegistration_Box"></a>

#### Declaration

```text
public FBox Box { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [FBox](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.FBox.html) |  |

### BoxUid <a id="FBoxClientDriver_Contract_Entity_BoxRegistration_BoxUid"></a>

#### Declaration

```text
public long BoxUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Group <a id="FBoxClientDriver_Contract_Entity_BoxRegistration_Group"></a>

#### Declaration

```text
[JsonProperty("group")]
public BoxGroupEntity Group { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxGroupEntity](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.BoxGroupEntity.html) |  |

### Id <a id="FBoxClientDriver_Contract_Entity_BoxRegistration_Id"></a>

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

