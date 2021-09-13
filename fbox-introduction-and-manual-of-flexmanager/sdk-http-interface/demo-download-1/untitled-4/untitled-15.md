# AddDataMonitorGroupArgs

新增监控点组别参数

#### Inheritance

System.Object

AddDataMonitorGroupArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_AddDataMonitorGroupArgs_syntax"></a>

```text
public class AddDataMonitorGroupArgs
```

## Constructors <a id="constructors"></a>

### AddDataMonitorGroupArgs\(\) <a id="FBoxClientDriver_Contract_AddDataMonitorGroupArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public AddDataMonitorGroupArgs()
```

### AddDataMonitorGroupArgs\(String, String\) <a id="FBoxClientDriver_Contract_AddDataMonitorGroupArgs__ctor_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public AddDataMonitorGroupArgs(string name, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name | 盒子检测点组名称 |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_AddDataMonitorGroupArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_AddDataMonitorGroupArgs_Name"></a>

盒子检测点组名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

