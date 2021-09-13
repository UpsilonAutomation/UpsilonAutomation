# BoxGroup

盒子组别

#### Inheritance

System.Object

BoxGroup

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

#### Syntax <a id="FBoxClientDriver_Contract_BoxGroup_syntax"></a>

## Constructors <a id="constructors"></a>

### BoxGroup\(\) <a id="FBoxClientDriver_Contract_BoxGroup__ctor"></a>

构造函数

#### Declaration

### BoxGroup\(Int64, String, IList\) <a id="FBoxClientDriver_Contract_BoxGroup__ctor_System_Int64_System_String_System_Collections_Generic_IList_FBoxClientDriver_Contract_Box__"></a>

构造函数

#### Declaration

```text
public BoxGroup(long uid, string name, IList boxes)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | uid | 盒子组别UID |
| System.String | name | 盒子组别名称 |
| System.Collections.Generic.IList&lt;[Box](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Box.html)&gt; | boxes | 盒子列表 |

## Properties <a id="properties"></a>

### Boxes <a id="FBoxClientDriver_Contract_BoxGroup_Boxes"></a>

盒子列表

#### Declaration

```text
public IList Boxes { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[Box](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Box.html)&gt; |  |

### Name <a id="FBoxClientDriver_Contract_BoxGroup_Name"></a>

盒子组别名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_BoxGroup_Uid"></a>

盒子组别UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

