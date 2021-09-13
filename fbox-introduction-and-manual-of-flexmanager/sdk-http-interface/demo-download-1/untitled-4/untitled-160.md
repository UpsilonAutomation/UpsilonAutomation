# UpdateBoxArgs

更新盒子参数

#### Inheritance

System.Object

UpdateBoxArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateBoxArgs_syntax"></a>

```text
public class UpdateBoxArgs
```

## Constructors <a id="constructors"></a>

### UpdateBoxArgs\(\) <a id="FBoxClientDriver_Contract_UpdateBoxArgs__ctor"></a>

无参构造函数

#### Declaration

### UpdateBoxArgs\(String, String\) <a id="FBoxClientDriver_Contract_UpdateBoxArgs__ctor_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public UpdateBoxArgs(string boxNo, string alias)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.String | alias |  |

## Properties <a id="properties"></a>

### Alias <a id="FBoxClientDriver_Contract_UpdateBoxArgs_Alias"></a>

盒子名称

#### Declaration

```text
public string Alias { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxNo <a id="FBoxClientDriver_Contract_UpdateBoxArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

