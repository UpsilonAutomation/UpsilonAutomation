# AlarmEventQuery2

历史数据查询参数

#### Inheritance

System.Object

AlarmEventQuery2

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

#### Syntax <a id="FBoxClientDriver_Contract_AlarmEventQuery2_syntax"></a>

```text
public class AlarmEventQuery2
```

## Constructors <a id="constructors"></a>

### AlarmEventQuery2\(\) <a id="FBoxClientDriver_Contract_AlarmEventQuery2__ctor"></a>

无参构造函数

#### Declaration

```text
public AlarmEventQuery2()
```

### AlarmEventQuery2\(String, IList, DateTime, DateTime, Int32\) <a id="FBoxClientDriver_Contract_AlarmEventQuery2__ctor_System_String_System_Collections_Generic_IList_System_Int64__System_DateTime_System_DateTime_System_Int32_"></a>

构造函数

#### Declaration

```text
public AlarmEventQuery2(string boxNo, IList ids, DateTime beginTime, DateTime endTime, int limit = 100)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo |  |
| System.Collections.Generic.IList&lt;System.Int64&gt; | ids | 历史数据定义ID列表 |
| System.DateTime | beginTime | 开始时间 |
| System.DateTime | endTime | 结束时间 |
| System.Int32 | limit | 查询条数 |

## Properties <a id="properties"></a>

### BeginTime <a id="FBoxClientDriver_Contract_AlarmEventQuery2_BeginTime"></a>

开始时间（包含此时间点）

#### Declaration

```text
public DateTime BeginTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### BoxNo <a id="FBoxClientDriver_Contract_AlarmEventQuery2_BoxNo"></a>

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### EndTime <a id="FBoxClientDriver_Contract_AlarmEventQuery2_EndTime"></a>

结束时间（不包含此时间点）

#### Declaration

```text
public DateTime EndTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### Ids <a id="FBoxClientDriver_Contract_AlarmEventQuery2_Ids"></a>

历史数据定义ID列表

#### Declaration

```text
public IList Ids { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; |  |

### Limit <a id="FBoxClientDriver_Contract_AlarmEventQuery2_Limit"></a>

查询条数

#### Declaration

```text
public int Limit { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

