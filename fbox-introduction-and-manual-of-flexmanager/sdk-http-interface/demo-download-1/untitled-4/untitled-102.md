# GetAlarmTargetArgs

获取单条报警联系人参数

#### Inheritance

System.Object

GetAlarmTargetArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_GetAlarmTargetArgs_syntax"></a>

```text
public class GetAlarmTargetArgs
```

## Constructors <a id="constructors"></a>

### GetAlarmTargetArgs\(\) <a id="FBoxClientDriver_Contract_GetAlarmTargetArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public GetAlarmTargetArgs()
```

### GetAlarmTargetArgs\(String, String\) <a id="FBoxClientDriver_Contract_GetAlarmTargetArgs__ctor_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public GetAlarmTargetArgs(string boxNo, string uid)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.String | uid | 报警联系人Uid |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_GetAlarmTargetArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_GetAlarmTargetArgs_Uid"></a>

报警联系人Uid

#### Declaration

```text
public string Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

