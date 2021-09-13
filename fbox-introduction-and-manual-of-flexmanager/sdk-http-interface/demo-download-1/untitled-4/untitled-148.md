# RemoveDataMonitorGroupArgs

移除监控点组别参数

#### Inheritance

System.Object

RemoveDataMonitorGroupArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_RemoveDataMonitorGroupArgs_syntax"></a>

```text
public class RemoveDataMonitorGroupArgs
```

## Constructors <a id="constructors"></a>

### RemoveDataMonitorGroupArgs\(\) <a id="FBoxClientDriver_Contract_RemoveDataMonitorGroupArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public RemoveDataMonitorGroupArgs()
```

### RemoveDataMonitorGroupArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_RemoveDataMonitorGroupArgs__ctor_System_String_System_Int64_"></a>

#### Declaration

```text
public RemoveDataMonitorGroupArgs(string boxNo, long groupUid)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | groupUid | 监测点组别UID |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_RemoveDataMonitorGroupArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### GroupUid <a id="FBoxClientDriver_Contract_RemoveDataMonitorGroupArgs_GroupUid"></a>

监测点组别UID

#### Declaration

```text
public long GroupUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

