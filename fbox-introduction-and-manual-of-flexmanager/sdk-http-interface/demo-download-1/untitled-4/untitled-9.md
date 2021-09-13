# AddHdataItemArgs

历史记录新增参数

#### Inheritance

System.Object

AddHdataItemArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_AddHdataItemArgs_syntax"></a>

```text
public class AddHdataItemArgs
```

## Constructors <a id="constructors"></a>

### AddHdataItemArgs\(\) <a id="FBoxClientDriver_Contract_AddHdataItemArgs__ctor"></a>

构造函数

#### Declaration

```text
public AddHdataItemArgs()
```

### AddHdataItemArgs\(String, IList\) <a id="FBoxClientDriver_Contract_AddHdataItemArgs__ctor_System_String_System_Collections_Generic_IList_FBoxClientDriver_Contract_AddHdataItemDto__"></a>

构造函数

#### Declaration

```text
public AddHdataItemArgs(string boxNo, IList hdataItems)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子号码 |
| System.Collections.Generic.IList&lt;[AddHdataItemDto](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHdataItemDto.html)&gt; | hdataItems | 多通道参数集合 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_AddHdataItemArgs_BoxNo"></a>

盒子号码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### HdataItems <a id="FBoxClientDriver_Contract_AddHdataItemArgs_HdataItems"></a>

多通道参数集合

#### Declaration

```text
public IList HdataItems { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[AddHdataItemDto](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHdataItemDto.html)&gt; |  |

