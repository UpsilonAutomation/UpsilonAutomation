# AlarmEventQuery

报警事件参数

#### Inheritance

System.Object

AlarmEventQuery

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

#### Syntax <a id="FBoxClientDriver_Contract_AlarmEventQuery_syntax"></a>

```text
public class AlarmEventQuery
```

## Constructors <a id="constructors"></a>

### AlarmEventQuery\(\) <a id="FBoxClientDriver_Contract_AlarmEventQuery__ctor"></a>

无参构造函数

#### Declaration

### AlarmEventQuery\(String, DateTime, DateTime, Int32, String\) <a id="FBoxClientDriver_Contract_AlarmEventQuery__ctor_System_String_System_DateTime_System_DateTime_System_Int32_System_String_"></a>

构造函数

#### Declaration

```text
public AlarmEventQuery(string boxNo, DateTime beginTime, DateTime endTime, int limit = 100, string name = null)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.DateTime | beginTime | 开始时间 |
| System.DateTime | endTime | 结束时间 |
| System.Int32 | limit | 查询条数 |
| System.String | name | 报警条目编码，若不为0，则查出指定编码的记录，否则不做限制 |

## Properties <a id="properties"></a>

### BeginTime <a id="FBoxClientDriver_Contract_AlarmEventQuery_BeginTime"></a>

开始时间（包含此时间点）

#### Declaration

```text
public DateTime BeginTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### BoxNo <a id="FBoxClientDriver_Contract_AlarmEventQuery_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Code <a id="FBoxClientDriver_Contract_AlarmEventQuery_Code"></a>

报警条目编码，若设置为0，则查所有条目的记录，若不为0，则查指定目记录

#### Declaration

```text
[JsonProperty("name")]
public string Code { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### EndTime <a id="FBoxClientDriver_Contract_AlarmEventQuery_EndTime"></a>

结束时间（不包含此时间点）

#### Declaration

```text
public DateTime EndTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### Limit <a id="FBoxClientDriver_Contract_AlarmEventQuery_Limit"></a>

查询条数

#### Declaration

```text
public int Limit { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Name <a id="FBoxClientDriver_Contract_AlarmEventQuery_Name"></a>

#### Declaration

```text
[JsonProperty("realname")]
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

