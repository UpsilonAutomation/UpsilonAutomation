# UpdateHdataItemArgs

历史记录更新参数

#### Inheritance

System.Object

UpdateHdataItemArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateHdataItemArgs_syntax"></a>

```text
public class UpdateHdataItemArgs
```

## Constructors <a id="constructors"></a>

### UpdateHdataItemArgs\(\) <a id="FBoxClientDriver_Contract_UpdateHdataItemArgs__ctor"></a>

构造函数

#### Declaration

```text
public UpdateHdataItemArgs()
```

### UpdateHdataItemArgs\(String, IList\) <a id="FBoxClientDriver_Contract_UpdateHdataItemArgs__ctor_System_String_System_Collections_Generic_IList_FBoxClientDriver_Contract_UpdateHdataItemDto__"></a>

构造函数

#### Declaration

```text
public UpdateHdataItemArgs(string boxNo, IList hdataItems)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子号码 |
| System.Collections.Generic.IList&lt;[UpdateHdataItemDto](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataItemDto.html)&gt; | hdataItems | 更新历史记录多通道参数System.Collections.Generic.IList |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_UpdateHdataItemArgs_BoxNo"></a>

盒子号码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### HdataItems <a id="FBoxClientDriver_Contract_UpdateHdataItemArgs_HdataItems"></a>

更新历史记录多通道参数

#### Declaration

```text
public IList HdataItems { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[UpdateHdataItemDto](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataItemDto.html)&gt; |  |

