# RemoveAlarmGroupArgs

移除报警组别参数

#### Inheritance

System.Object

RemoveAlarmGroupArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_RemoveAlarmGroupArgs_syntax"></a>

```text
public class RemoveAlarmGroupArgs
```

## Constructors <a id="constructors"></a>

### RemoveAlarmGroupArgs\(\) <a id="FBoxClientDriver_Contract_RemoveAlarmGroupArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public RemoveAlarmGroupArgs()
```

### RemoveAlarmGroupArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_RemoveAlarmGroupArgs__ctor_System_String_System_Int64_"></a>

构造函数

#### Declaration

```text
public RemoveAlarmGroupArgs(string boxNo, long uid)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | uid | 报警组UID |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_RemoveAlarmGroupArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_RemoveAlarmGroupArgs_Uid"></a>

报警组UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

