# BoxRegisterArgs

盒子注册事件参数

#### Inheritance

System.Object

System.EventArgs

BoxRegisterArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_BoxRegisterArgs_syntax"></a>

```text
public class BoxRegisterArgs : EventArgs
```

## Constructors <a id="constructors"></a>

### BoxRegisterArgs\(String, String, String\) <a id="FBoxClientDriver_Contract_BoxRegisterArgs__ctor_System_String_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public BoxRegisterArgs(string boxNo, string boxId, string name)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.String | boxId | 盒子Id |
| System.String | name | 名称 |

## Properties <a id="properties"></a>

### BoxId <a id="FBoxClientDriver_Contract_BoxRegisterArgs_BoxId"></a>

盒子Id

#### Declaration

```text
public string BoxId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxNo <a id="FBoxClientDriver_Contract_BoxRegisterArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_BoxRegisterArgs_Name"></a>

名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

