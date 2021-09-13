# AddAlarmGroupArgs

新增报警组别参数

#### Inheritance

System.Object

AddAlarmGroupArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_AddAlarmGroupArgs_syntax"></a>

```text
public class AddAlarmGroupArgs
```

## Constructors <a id="constructors"></a>

### AddAlarmGroupArgs\(\) <a id="FBoxClientDriver_Contract_AddAlarmGroupArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public AddAlarmGroupArgs()
```

### AddAlarmGroupArgs\(String, String, String\) <a id="FBoxClientDriver_Contract_AddAlarmGroupArgs__ctor_System_String_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public AddAlarmGroupArgs(string boxNo, string name, string memo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.String | name | 报警组名称 |
| System.String | memo | 报警组备注 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_AddAlarmGroupArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Memo <a id="FBoxClientDriver_Contract_AddAlarmGroupArgs_Memo"></a>

报警组备注

#### Declaration

```text
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_AddAlarmGroupArgs_Name"></a>

报警组名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

