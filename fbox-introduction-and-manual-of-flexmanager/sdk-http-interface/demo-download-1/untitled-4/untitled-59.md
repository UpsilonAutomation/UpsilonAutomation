# DataMonitorPointArgs

设置单个监测点开启/停止参数

#### Inheritance

System.Object

DataMonitorPointArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_DataMonitorPointArgs_syntax"></a>

```text
public class DataMonitorPointArgs
```

## Constructors <a id="constructors"></a>

### DataMonitorPointArgs\(\) <a id="FBoxClientDriver_Contract_DataMonitorPointArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public DataMonitorPointArgs()
```

### DataMonitorPointArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_DataMonitorPointArgs__ctor_System_String_System_Int64_"></a>

#### Declaration

```text
public DataMonitorPointArgs(string boxNo, long dataMonitorUid)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | dataMonitorUid | 监测点UID |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_DataMonitorPointArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataMonitorUid <a id="FBoxClientDriver_Contract_DataMonitorPointArgs_DataMonitorUid"></a>

监测点UID

#### Declaration

```text
public long DataMonitorUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

