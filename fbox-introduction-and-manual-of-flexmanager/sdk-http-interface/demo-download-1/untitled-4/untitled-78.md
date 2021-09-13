# GetHDataArgs

获取历史记录参数

#### Inheritance

System.Object

GetHDataArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_GetHDataArgs_syntax"></a>

```text
public class GetHDataArgs
```

## Constructors <a id="constructors"></a>

### GetHDataArgs\(\) <a id="FBoxClientDriver_Contract_GetHDataArgs__ctor"></a>

构造函数

#### Declaration

### GetHDataArgs\(String, Int64, DataType, DateTime, DateTime, Int32\) <a id="FBoxClientDriver_Contract_GetHDataArgs__ctor_System_String_System_Int64_FBoxClientDriver_Contract_DataType_System_DateTime_System_DateTime_System_Int32_"></a>

构造函数

#### Declaration

```text
public GetHDataArgs(string boxNo, long uid, DataType dataType, DateTime startTime, DateTime endTime, int maxCount)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | uid | 历史条目UID |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 |
| System.DateTime | startTime | 起始时间 |
| System.DateTime | endTime | 结束时间 |
| System.Int32 | maxCount | 最大获取条数 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_GetHDataArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataType <a id="FBoxClientDriver_Contract_GetHDataArgs_DataType"></a>

#### Declaration

```text
public DataType DataType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### EndTime <a id="FBoxClientDriver_Contract_GetHDataArgs_EndTime"></a>

结束时间

#### Declaration

```text
public DateTime EndTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### MaxCount <a id="FBoxClientDriver_Contract_GetHDataArgs_MaxCount"></a>

最大获取条数

#### Declaration

```text
public int MaxCount { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StartTime <a id="FBoxClientDriver_Contract_GetHDataArgs_StartTime"></a>

开始时间

#### Declaration

```text
public DateTime StartTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### Uid <a id="FBoxClientDriver_Contract_GetHDataArgs_Uid"></a>

历史条目Uid

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

