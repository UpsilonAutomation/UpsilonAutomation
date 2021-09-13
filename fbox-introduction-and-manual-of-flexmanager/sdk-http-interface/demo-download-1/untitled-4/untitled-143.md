# RemoveAlarmDefinitionArgs

删除报警条目参数

#### Inheritance

System.Object

RemoveAlarmDefinitionArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_RemoveAlarmDefinitionArgs_syntax"></a>

```text
public class RemoveAlarmDefinitionArgs
```

## Constructors <a id="constructors"></a>

### RemoveAlarmDefinitionArgs\(\) <a id="FBoxClientDriver_Contract_RemoveAlarmDefinitionArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public RemoveAlarmDefinitionArgs()
```

### RemoveAlarmDefinitionArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_RemoveAlarmDefinitionArgs__ctor_System_String_System_Int64_"></a>

构造函数

#### Declaration

```text
public RemoveAlarmDefinitionArgs(string boxNo, long alarmDefUid)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | alarmDefUid | 报警条目UID |

## Properties <a id="properties"></a>

### AlarmDefUid <a id="FBoxClientDriver_Contract_RemoveAlarmDefinitionArgs_AlarmDefUid"></a>

报警条目UID

#### Declaration

```text
public long AlarmDefUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### BoxNo <a id="FBoxClientDriver_Contract_RemoveAlarmDefinitionArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

