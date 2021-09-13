# GetDmonDataSourceIdArgs

获取监控点下发Id参数

#### Inheritance

System.Object

GetDmonDataSourceIdArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_GetDmonDataSourceIdArgs_syntax"></a>

```text
public class GetDmonDataSourceIdArgs
```

## Constructors <a id="constructors"></a>

### GetDmonDataSourceIdArgs\(\) <a id="FBoxClientDriver_Contract_GetDmonDataSourceIdArgs__ctor"></a>

构造函数

#### Declaration

```text
public GetDmonDataSourceIdArgs()
```

### GetDmonDataSourceIdArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_GetDmonDataSourceIdArgs__ctor_System_String_System_Int64_"></a>

构造函数

#### Declaration

```text
public GetDmonDataSourceIdArgs(string boxNo, long dmonId)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | dmonId | 监控点条目Id |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_GetDmonDataSourceIdArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DmonId <a id="FBoxClientDriver_Contract_GetDmonDataSourceIdArgs_DmonId"></a>

监控点条目Id

#### Declaration

```text
public long DmonId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

