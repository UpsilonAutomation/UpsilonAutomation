# BoxStateEntity

盒子状态更新

#### Inheritance

System.Object

BoxStateEntity

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

#### Syntax <a id="FBoxClientDriver_Contract_BoxStateEntity_syntax"></a>

```text
public class BoxStateEntity
```

## Constructors <a id="constructors"></a>

### BoxStateEntity\(\) <a id="FBoxClientDriver_Contract_BoxStateEntity__ctor"></a>

Constructor

#### Declaration

### BoxStateEntity\(String, BoxConnectionState\) <a id="FBoxClientDriver_Contract_BoxStateEntity__ctor_System_String_FBoxClientDriver_Contract_BoxConnectionState_"></a>

Constructor

#### Declaration

```text
public BoxStateEntity(string boxNo, BoxConnectionState state)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) | state | 盒子状态 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_BoxStateEntity_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### State <a id="FBoxClientDriver_Contract_BoxStateEntity_State"></a>

盒子状态

#### Declaration

```text
public BoxConnectionState State { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) |  |

