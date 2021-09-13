# UpdateDataMonitorGroupArgs

更新盒子监测点组参数

#### Inheritance

System.Object

UpdateDataMonitorGroupArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateDataMonitorGroupArgs_syntax"></a>

```text
public class UpdateDataMonitorGroupArgs
```

## Constructors <a id="constructors"></a>

### UpdateDataMonitorGroupArgs\(\) <a id="FBoxClientDriver_Contract_UpdateDataMonitorGroupArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public UpdateDataMonitorGroupArgs()
```

### UpdateDataMonitorGroupArgs\(Int64, String, String\) <a id="FBoxClientDriver_Contract_UpdateDataMonitorGroupArgs__ctor_System_Int64_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public UpdateDataMonitorGroupArgs(long uid, string name, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | uid | 盒子监测点组UID |
| System.String | name | 盒子检测点组名称 |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_UpdateDataMonitorGroupArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_UpdateDataMonitorGroupArgs_Name"></a>

盒子检测点组名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_UpdateDataMonitorGroupArgs_Uid"></a>

盒子监测点组UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

