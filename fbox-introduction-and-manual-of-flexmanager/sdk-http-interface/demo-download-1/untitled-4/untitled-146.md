# RemoveDataMonDefArgsV2

删除数据监控条目参数

#### Inheritance

System.Object

RemoveDataMonDefArgsV2

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

#### Syntax <a id="FBoxClientDriver_Contract_RemoveDataMonDefArgsV2_syntax"></a>

```text
public class RemoveDataMonDefArgsV2
```

## Constructors <a id="constructors"></a>

### RemoveDataMonDefArgsV2\(\) <a id="FBoxClientDriver_Contract_RemoveDataMonDefArgsV2__ctor"></a>

构造函数

#### Declaration

```text
public RemoveDataMonDefArgsV2()
```

### RemoveDataMonDefArgsV2\(IList, String\) <a id="FBoxClientDriver_Contract_RemoveDataMonDefArgsV2__ctor_System_Collections_Generic_IList_System_Int64__System_String_"></a>

构造函数

#### Declaration

```text
public RemoveDataMonDefArgsV2(IList ids, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; | ids | 要删除的实时数据监控条目ID列表 |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_RemoveDataMonDefArgsV2_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Ids <a id="FBoxClientDriver_Contract_RemoveDataMonDefArgsV2_Ids"></a>

Id列表

#### Declaration

```text
public IList Ids { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; |  |

