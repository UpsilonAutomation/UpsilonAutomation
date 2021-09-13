# GetSomeDmonItemsArgsV2

获取某些实时数据条目参数

#### Inheritance

System.Object

GetSomeDmonItemsArgsV2

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

#### Syntax <a id="FBoxClientDriver_Contract_GetSomeDmonItemsArgsV2_syntax"></a>

```text
public class GetSomeDmonItemsArgsV2
```

## Constructors <a id="constructors"></a>

### GetSomeDmonItemsArgsV2\(\) <a id="FBoxClientDriver_Contract_GetSomeDmonItemsArgsV2__ctor"></a>

构造函数

#### Declaration

```text
public GetSomeDmonItemsArgsV2()
```

### GetSomeDmonItemsArgsV2\(IList, String\) <a id="FBoxClientDriver_Contract_GetSomeDmonItemsArgsV2__ctor_System_Collections_Generic_IList_System_Int64__System_String_"></a>

构造函数

#### Declaration

```text
public GetSomeDmonItemsArgsV2(IList ids, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; | ids | 实时数据条目ID列表 |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_GetSomeDmonItemsArgsV2_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Ids <a id="FBoxClientDriver_Contract_GetSomeDmonItemsArgsV2_Ids"></a>

实时数据条目ID列表

#### Declaration

```text
public IList Ids { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; |  |

