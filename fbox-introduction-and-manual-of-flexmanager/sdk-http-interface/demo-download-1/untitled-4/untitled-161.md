# UpdateBoxGroupArgs

盒子组别参数

#### Inheritance

System.Object

UpdateBoxGroupArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateBoxGroupArgs_syntax"></a>

```text
public class UpdateBoxGroupArgs
```

## Constructors <a id="constructors"></a>

### UpdateBoxGroupArgs\(\) <a id="FBoxClientDriver_Contract_UpdateBoxGroupArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public UpdateBoxGroupArgs()
```

### UpdateBoxGroupArgs\(Int64, String\) <a id="FBoxClientDriver_Contract_UpdateBoxGroupArgs__ctor_System_Int64_System_String_"></a>

构造函数

#### Declaration

```text
public UpdateBoxGroupArgs(long uid, string name)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | uid | 盒子组别UID |
| System.String | name | 盒子组别名称 |

## Properties <a id="properties"></a>

### Name <a id="FBoxClientDriver_Contract_UpdateBoxGroupArgs_Name"></a>

盒子组别名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_UpdateBoxGroupArgs_Uid"></a>

盒子组别UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

