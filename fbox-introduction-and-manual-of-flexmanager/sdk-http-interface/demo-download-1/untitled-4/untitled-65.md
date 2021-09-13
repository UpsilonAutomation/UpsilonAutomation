# DataMonitorWriteValueArgsV2

写入值参数

#### Inheritance

System.Object

DataMonitorWriteValueArgsV2

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

#### Syntax <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2_syntax"></a>

```text
public class DataMonitorWriteValueArgsV2
```

## Constructors <a id="constructors"></a>

### DataMonitorWriteValueArgsV2\(\) <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2__ctor"></a>

无参构造函数

#### Declaration

```text
public DataMonitorWriteValueArgsV2()
```

### DataMonitorWriteValueArgsV2\(String, Int64, Object, WriteValueType\) <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2__ctor_System_String_System_Int64_System_Object_FBoxClientDriver_Contract_WriteValueType_"></a>

构造函数

#### Declaration

```text
public DataMonitorWriteValueArgsV2(string boxNo, long dataMonitorUid, object value, WriteValueType type)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | dataMonitorUid | 监测点条目UID |
| System.Object | value | 检测点条目的值 |
| [WriteValueType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.WriteValueType.html) | type | 监测点条目值类型 |

### DataMonitorWriteValueArgsV2\(String, String, Object, WriteValueType\) <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2__ctor_System_String_System_String_System_Object_FBoxClientDriver_Contract_WriteValueType_"></a>

构造函数

#### Declaration

```text
public DataMonitorWriteValueArgsV2(string boxNo, string dataMonitorName, object value, WriteValueType type)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.String | dataMonitorName | 监控点名称 |
| System.Object | value | 检测点条目的值 |
| [WriteValueType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.WriteValueType.html) | type | 监测点条目值类型 |

### DataMonitorWriteValueArgsV2\(String, String, String, Object, WriteValueType\) <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2__ctor_System_String_System_String_System_String_System_Object_FBoxClientDriver_Contract_WriteValueType_"></a>

构造函数

#### Declaration

```text
public DataMonitorWriteValueArgsV2(string boxNo, string dataMonitorName, string dataMonitorGroupName, object value, WriteValueType type)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.String | dataMonitorName | 监控点名称 |
| System.String | dataMonitorGroupName | 监控点组名称，用于不同组下有同名监控点的情况。 |
| System.Object | value | 检测点条目的值 |
| [WriteValueType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.WriteValueType.html) | type | 监测点条目值类型 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataMonitorGroupName <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2_DataMonitorGroupName"></a>

监控点组名称

#### Declaration

```text
public string DataMonitorGroupName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataMonitorName <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2_DataMonitorName"></a>

监控点条目名称

#### Declaration

```text
public string DataMonitorName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataMonitorUid <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2_DataMonitorUid"></a>

监测点条目UID

#### Declaration

```text
public long DataMonitorUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Type <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2_Type"></a>

监测点条目值类型

#### Declaration

```text
public WriteValueType Type { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [WriteValueType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.WriteValueType.html) |  |

### Value <a id="FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2_Value"></a>

检测点条目的值

#### Declaration

```text
public object Value { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Object |  |

