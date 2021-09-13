# DataMonitorWriteValueArgs

写入值参数

#### Inheritance

System.Object

DataMonitorWriteValueArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgs_syntax"></a>

```text
public class DataMonitorWriteValueArgs
```

## Constructors <a id="constructors"></a>

### DataMonitorWriteValueArgs\(\) <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public DataMonitorWriteValueArgs()
```

### DataMonitorWriteValueArgs\(String, Int64, Object, WriteValueType\) <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgs__ctor_System_String_System_Int64_System_Object_FBoxClientDriver_Contract_WriteValueType_"></a>

构造函数

#### Declaration

```text
public DataMonitorWriteValueArgs(string boxNo, long dataMonitorUid, object value, WriteValueType type)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | dataMonitorUid | 监测点条目UID |
| System.Object | value | 检测点条目的值 |
| [WriteValueType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.WriteValueType.html) | type | 监测点条目值类型 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataMonitorUid <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgs_DataMonitorUid"></a>

监测点条目UID

#### Declaration

```text
public long DataMonitorUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Type <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgs_Type"></a>

监测点条目值类型

#### Declaration

```text
public WriteValueType Type { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [WriteValueType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.WriteValueType.html) |  |

### Value <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgs_Value"></a>

检测点条目的值

#### Declaration

```text
public object Value { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Object |  |

