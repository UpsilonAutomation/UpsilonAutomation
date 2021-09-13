# DataMonitorGroupsArgs

设置监测点开启数据推送参数

#### Inheritance

System.Object

DataMonitorGroupsArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_DataMonitorGroupsArgs_syntax"></a>

```text
public class DataMonitorGroupsArgs
```

## Constructors <a id="constructors"></a>

### DataMonitorGroupsArgs\(\) <a id="FBoxClientDriver_Contract_DataMonitorGroupsArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public DataMonitorGroupsArgs()
```

### DataMonitorGroupsArgs\(String, IList\) <a id="FBoxClientDriver_Contract_DataMonitorGroupsArgs__ctor_System_String_System_Collections_Generic_IList_System_Int64__"></a>

构造函数

#### Declaration

```text
public DataMonitorGroupsArgs(string boxNo, IList dataMonitorGroupList)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Collections.Generic.IList&lt;System.Int64&gt; | dataMonitorGroupList | 检测点组别列表 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_DataMonitorGroupsArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DataMonitorGroupList <a id="FBoxClientDriver_Contract_DataMonitorGroupsArgs_DataMonitorGroupList"></a>

监控点组别数据列表

#### Declaration

```text
public IList DataMonitorGroupList { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; |  |

