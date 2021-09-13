# DataMonitorGroupArgs

设置监控点组别开始/停止参数

#### Inheritance

System.Object

DataMonitorGroupArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_DataMonitorGroupArgs_syntax"></a>

```text
public class DataMonitorGroupArgs
```

## Constructors <a id="constructors"></a>

### DataMonitorGroupArgs\(\) <a id="FBoxClientDriver_Contract_DataMonitorGroupArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public DataMonitorGroupArgs()
```

### DataMonitorGroupArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_DataMonitorGroupArgs__ctor_System_String_System_Int64_"></a>

构造函数

#### Declaration

```text
public DataMonitorGroupArgs(string boxNo, long dataMonitorGroupUid)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | dataMonitorGroupUid | 监测点组UID |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_DataMonitorGroupArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataMonitorGroupUid <a id="FBoxClientDriver_Contract_DataMonitorGroupArgs_DataMonitorGroupUid"></a>

监测点组UID

#### Declaration

```text
public long DataMonitorGroupUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

