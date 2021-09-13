# DataMonitorPointsByGroupedNameArgs

设备监控点启用/停止参数

#### Inheritance

System.Object

DataMonitorPointsByGroupedNameArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_DataMonitorPointsByGroupedNameArgs_syntax"></a>

```text
public class DataMonitorPointsByGroupedNameArgs
```

## Constructors <a id="constructors"></a>

### DataMonitorPointsByGroupedNameArgs\(\) <a id="FBoxClientDriver_Contract_DataMonitorPointsByGroupedNameArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public DataMonitorPointsByGroupedNameArgs()
```

### DataMonitorPointsByGroupedNameArgs\(IDictionary&gt;, String\) <a id="FBoxClientDriver_Contract_DataMonitorPointsByGroupedNameArgs__ctor_System_Collections_Generic_IDictionary_System_String_System_Collections_Generic_IList_System_String___System_String_"></a>

构造函数

#### Declaration

```text
public DataMonitorPointsByGroupedNameArgs(IDictionary> dataMonitorList, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IDictionary&lt;System.String, System.Collections.Generic.IList&lt;System.String&gt;&gt; | dataMonitorList | 监测点列 |
| System.String | boxNo | 盒子编码 |

### DataMonitorPointsByGroupedNameArgs\(IEnumerable&gt;, String\) <a id="FBoxClientDriver_Contract_DataMonitorPointsByGroupedNameArgs__ctor_System_Collections_Generic_IEnumerable_System_Tuple_System_String_System_String___System_String_"></a>

构造函数

#### Declaration

```text
public DataMonitorPointsByGroupedNameArgs(IEnumerable> dataMonitorList, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IEnumerable&lt;System.Tuple&lt;System.String, System.String&gt;&gt; | dataMonitorList | 监测点列表\(name, groupName\) |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_DataMonitorPointsByGroupedNameArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataMonitorList <a id="FBoxClientDriver_Contract_DataMonitorPointsByGroupedNameArgs_DataMonitorList"></a>

监测点列表

#### Declaration

```text
public IDictionary> DataMonitorList { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IDictionary&lt;System.String, System.Collections.Generic.IList&lt;System.String&gt;&gt; |  |

