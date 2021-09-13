# StartDmonItemByNamesArgs

根据名称开启点参数

#### Inheritance

System.Object

StartDmonItemByNamesArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_StartDmonItemByNamesArgs_syntax"></a>

```text
public class StartDmonItemByNamesArgs
```

## Constructors <a id="constructors"></a>

### StartDmonItemByNamesArgs\(\) <a id="FBoxClientDriver_Contract_StartDmonItemByNamesArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public StartDmonItemByNamesArgs()
```

### StartDmonItemByNamesArgs\(String, String\[\]\) <a id="FBoxClientDriver_Contract_StartDmonItemByNamesArgs__ctor_System_String_System_String___"></a>

构造函数

#### Declaration

```text
public StartDmonItemByNamesArgs(string boxNo, string[] names)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子号码 |
| System.String\[\] | names | 名称列表 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_StartDmonItemByNamesArgs_BoxNo"></a>

盒子号码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Names <a id="FBoxClientDriver_Contract_StartDmonItemByNamesArgs_Names"></a>

名称列表

#### Declaration

```text
public string[] Names { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String\[\] |  |

