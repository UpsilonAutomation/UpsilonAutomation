# AddHdataDefArgsV2

新增历史条目参数

#### Inheritance

System.Object

AddHdataDefArgsV2

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

#### Syntax <a id="FBoxClientDriver_Contract_AddHdataDefArgsV2_syntax"></a>

```text
public class AddHdataDefArgsV2
```

## Constructors <a id="constructors"></a>

### AddHdataDefArgsV2\(\) <a id="FBoxClientDriver_Contract_AddHdataDefArgsV2__ctor"></a>

构造函数

#### Declaration

```text
public AddHdataDefArgsV2()
```

### AddHdataDefArgsV2\(IList, String\) <a id="FBoxClientDriver_Contract_AddHdataDefArgsV2__ctor_System_Collections_Generic_IList_FBoxClientDriver_Contract_AddHdataDefinitionV2__System_String_"></a>

构造函数

#### Declaration

```text
public AddHdataDefArgsV2(IList addHdatas, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IList&lt;[AddHdataDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHdataDefinitionV2.html)&gt; | addHdatas | 历史条目列表 |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### AddHdatas <a id="FBoxClientDriver_Contract_AddHdataDefArgsV2_AddHdatas"></a>

#### Declaration

```text
public IList AddHdatas { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[AddHdataDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHdataDefinitionV2.html)&gt; |  |

### BoxNo <a id="FBoxClientDriver_Contract_AddHdataDefArgsV2_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

