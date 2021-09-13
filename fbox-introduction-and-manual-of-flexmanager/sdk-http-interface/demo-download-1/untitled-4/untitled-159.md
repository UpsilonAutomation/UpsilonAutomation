# UpdateAlarmGroupArgs

更新报警组别参数

#### Inheritance

System.Object

UpdateAlarmGroupArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateAlarmGroupArgs_syntax"></a>

```text
public class UpdateAlarmGroupArgs
```

## Constructors <a id="constructors"></a>

### UpdateAlarmGroupArgs\(\) <a id="FBoxClientDriver_Contract_UpdateAlarmGroupArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public UpdateAlarmGroupArgs()
```

### UpdateAlarmGroupArgs\(Int64, String, String\) <a id="FBoxClientDriver_Contract_UpdateAlarmGroupArgs__ctor_System_Int64_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public UpdateAlarmGroupArgs(long uid, string name, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | uid | 报警组UID |
| System.String | name | 报警组名称 |
| System.String | boxNo | 备注 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_UpdateAlarmGroupArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Memo <a id="FBoxClientDriver_Contract_UpdateAlarmGroupArgs_Memo"></a>

备注

#### Declaration

```text
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_UpdateAlarmGroupArgs_Name"></a>

报警组名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_UpdateAlarmGroupArgs_Uid"></a>

报警组UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

