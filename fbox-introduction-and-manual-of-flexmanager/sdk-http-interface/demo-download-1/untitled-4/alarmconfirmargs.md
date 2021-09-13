# AlarmConfirmArgs

确认报警参数

#### Inheritance

System.Object

AlarmConfirmArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_AlarmConfirmArgs_syntax"></a>

```text
public class AlarmConfirmArgs
```

## Constructors <a id="constructors"></a>

### AlarmConfirmArgs\(\) <a id="FBoxClientDriver_Contract_AlarmConfirmArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public AlarmConfirmArgs()
```

### AlarmConfirmArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_AlarmConfirmArgs__ctor_System_String_System_Int64_"></a>

构造函数

#### Declaration

```text
public AlarmConfirmArgs(string boxNo, long alarmUid)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | alarmUid | 报警条目Id |

## Properties <a id="properties"></a>

### AlarmUid <a id="FBoxClientDriver_Contract_AlarmConfirmArgs_AlarmUid"></a>

报警条目Id

#### Declaration

```text
public long AlarmUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### BoxNo <a id="FBoxClientDriver_Contract_AlarmConfirmArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

