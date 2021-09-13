# SetDataMonitorGroupOnlyArgs

设置监控点组别开始/停止参数

#### Inheritance

System.Object

SetDataMonitorGroupOnlyArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_SetDataMonitorGroupOnlyArgs_syntax"></a>

```text
public class SetDataMonitorGroupOnlyArgs
```

## Constructors <a id="constructors"></a>

### SetDataMonitorGroupOnlyArgs\(\) <a id="FBoxClientDriver_Contract_SetDataMonitorGroupOnlyArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public SetDataMonitorGroupOnlyArgs()
```

### SetDataMonitorGroupOnlyArgs\(String, IList\) <a id="FBoxClientDriver_Contract_SetDataMonitorGroupOnlyArgs__ctor_System_String_System_Collections_Generic_IList_System_Int64__"></a>

构造函数

#### Declaration

```text
public SetDataMonitorGroupOnlyArgs(string boxNo, IList dataMonitorGroupList)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Collections.Generic.IList&lt;System.Int64&gt; | dataMonitorGroupList | 监测点组UID |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_SetDataMonitorGroupOnlyArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataMonitorGroupList <a id="FBoxClientDriver_Contract_SetDataMonitorGroupOnlyArgs_DataMonitorGroupList"></a>

监测点组UID

#### Declaration

```text
public IList DataMonitorGroupList { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; |  |

