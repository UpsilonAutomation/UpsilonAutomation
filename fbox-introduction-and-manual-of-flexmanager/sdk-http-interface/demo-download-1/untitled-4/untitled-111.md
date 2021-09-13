# DMonRegisterArgs

注册监控点事件参数

#### Inheritance

System.Object

System.EventArgs

DMonRegisterArgs

#### Inherited Members

System.EventArgs.Empty

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver.Contract**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_DMonRegisterArgs_syntax"></a>

```text
public class DMonRegisterArgs : EventArgs
```

## Constructors <a id="constructors"></a>

### DMonRegisterArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_DMonRegisterArgs__ctor_System_String_System_Int64_"></a>

构造函数

#### Declaration

```text
public DMonRegisterArgs(string boxNo, long dMondefUid)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子UID |
| System.Int64 | dMondefUid | 监控点uid |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_DMonRegisterArgs_BoxNo"></a>

盒子UID

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DMondefUid <a id="FBoxClientDriver_Contract_DMonRegisterArgs_DMondefUid"></a>

监控点uid

#### Declaration

```text
public long DMondefUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

