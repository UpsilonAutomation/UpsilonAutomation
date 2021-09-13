# ChangeBoxGroupArgs

更换盒子组别参数

#### Inheritance

System.Object

ChangeBoxGroupArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_ChangeBoxGroupArgs_syntax"></a>

```text
public class ChangeBoxGroupArgs
```

## Constructors <a id="constructors"></a>

### ChangeBoxGroupArgs\(\) <a id="FBoxClientDriver_Contract_ChangeBoxGroupArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public ChangeBoxGroupArgs()
```

### ChangeBoxGroupArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_ChangeBoxGroupArgs__ctor_System_String_System_Int64_"></a>

构造函数

#### Declaration

```text
public ChangeBoxGroupArgs(string boxNo, long groupId)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | groupId | 盒子组Id |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_ChangeBoxGroupArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### GroupId <a id="FBoxClientDriver_Contract_ChangeBoxGroupArgs_GroupId"></a>

盒子组Id

#### Declaration

```text
public long GroupId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

