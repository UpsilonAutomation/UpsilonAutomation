# DMonDefUnregisterArgs

移除监控点事件参数

#### Inheritance

System.Object

DMonDefUnregisterArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_DMonDefUnregisterArgs_syntax"></a>

```text
public class DMonDefUnregisterArgs
```

## Constructors <a id="constructors"></a>

### DMonDefUnregisterArgs\(String, ICollection\) <a id="FBoxClientDriver_Contract_DMonDefUnregisterArgs__ctor_System_String_System_Collections_Generic_ICollection_System_Int64__"></a>

构造函数

#### Declaration

```text
public DMonDefUnregisterArgs(string boxNo, ICollection dMonDefList)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Collections.Generic.ICollection&lt;System.Int64&gt; | dMonDefList | 监控点集合 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_DMonDefUnregisterArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DMonDefList <a id="FBoxClientDriver_Contract_DMonDefUnregisterArgs_DMonDefList"></a>

监控点集合

#### Declaration

```text
public ICollection DMonDefList { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.ICollection&lt;System.Int64&gt; |  |

