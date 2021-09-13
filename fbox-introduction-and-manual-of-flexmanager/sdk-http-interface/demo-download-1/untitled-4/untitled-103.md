# GetAlarmDefinitionArgs

获取报警信息参数

#### Inheritance

System.Object

GetAlarmDefinitionArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_GetAlarmDefinitionArgs_syntax"></a>

```text
public class GetAlarmDefinitionArgs
```

## Constructors <a id="constructors"></a>

### GetAlarmDefinitionArgs\(\) <a id="FBoxClientDriver_Contract_GetAlarmDefinitionArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public GetAlarmDefinitionArgs()
```

### GetAlarmDefinitionArgs\(Int64, String\) <a id="FBoxClientDriver_Contract_GetAlarmDefinitionArgs__ctor_System_Int64_System_String_"></a>

构造函数

#### Declaration

```text
public GetAlarmDefinitionArgs(long uid, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | uid | 报警条目UID |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_GetAlarmDefinitionArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_GetAlarmDefinitionArgs_Uid"></a>

报警条目UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

