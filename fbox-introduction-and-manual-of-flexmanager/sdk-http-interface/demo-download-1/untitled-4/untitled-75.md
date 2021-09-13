# DMonEntry

实时数据类

#### Inheritance

System.Object

DMonEntry

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

#### Syntax <a id="FBoxClientDriver_Contract_DMonEntry_syntax"></a>

## Properties <a id="properties"></a>

### BoxId <a id="FBoxClientDriver_Contract_DMonEntry_BoxId"></a>

盒子ID

#### Declaration

```text
public long BoxId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### BoxNo <a id="FBoxClientDriver_Contract_DMonEntry_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataType <a id="FBoxClientDriver_Contract_DMonEntry_DataType"></a>

数据类型

#### Declaration

```text
public DataType DataType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### Id <a id="FBoxClientDriver_Contract_DMonEntry_Id"></a>

监控点ID

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Name <a id="FBoxClientDriver_Contract_DMonEntry_Name"></a>

监控点名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Status <a id="FBoxClientDriver_Contract_DMonEntry_Status"></a>

监控点状态

#### Declaration

```text
public DMonStatus Status { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DMonStatus](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DMonStatus.html) |  |

### Timestamp <a id="FBoxClientDriver_Contract_DMonEntry_Timestamp"></a>

时间戳，由于从缓存里拉的数据，所以需要时间戳来判断是否已经过期,UTC时间

#### Declaration

```text
public DateTime Timestamp { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### Value <a id="FBoxClientDriver_Contract_DMonEntry_Value"></a>

值

#### Declaration

```text
public object Value { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Object |  |

