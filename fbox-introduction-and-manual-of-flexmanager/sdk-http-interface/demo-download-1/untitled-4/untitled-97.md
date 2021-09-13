# GetDataMonitorDefArgs

获取数据监控点参数

#### Inheritance

System.Object

GetDataMonitorDefArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_GetDataMonitorDefArgs_syntax"></a>

```text
public class GetDataMonitorDefArgs
```

## Constructors <a id="constructors"></a>

### GetDataMonitorDefArgs\(\) <a id="FBoxClientDriver_Contract_GetDataMonitorDefArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public GetDataMonitorDefArgs()
```

### GetDataMonitorDefArgs\(String, Int64\) <a id="FBoxClientDriver_Contract_GetDataMonitorDefArgs__ctor_System_String_System_Int64_"></a>

构造函数

#### Declaration

```text
public GetDataMonitorDefArgs(string boxNo, long uid)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int64 | uid | 监测点条目UID |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_GetDataMonitorDefArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_GetDataMonitorDefArgs_Uid"></a>

监测点条目UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

