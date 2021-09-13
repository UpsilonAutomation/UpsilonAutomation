# GetDMonitorGroupArgs

获取单条监测点组参数

#### Inheritance

System.Object

GetDMonitorGroupArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_GetDMonitorGroupArgs_syntax"></a>

```text
public class GetDMonitorGroupArgs
```

## Constructors <a id="constructors"></a>

### GetDMonitorGroupArgs\(\) <a id="FBoxClientDriver_Contract_GetDMonitorGroupArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public GetDMonitorGroupArgs()
```

### GetDMonitorGroupArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_GetDMonitorGroupArgs__ctor_System_String_System_Int64_"></a>

构造函数

#### Declaration

```text
public GetDMonitorGroupArgs(string boxNo, long uid)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | uid | 检测点组别UID |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_GetDMonitorGroupArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_GetDMonitorGroupArgs_Uid"></a>

检测点组别UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

