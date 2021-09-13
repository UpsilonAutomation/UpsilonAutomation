# UpdateHdataDefArgsV2

更新历史记录参数

#### Inheritance

System.Object

UpdateHdataDefArgsV2

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateHdataDefArgsV2_syntax"></a>

```text
public class UpdateHdataDefArgsV2
```

## Constructors <a id="constructors"></a>

### UpdateHdataDefArgsV2\(\) <a id="FBoxClientDriver_Contract_UpdateHdataDefArgsV2__ctor"></a>

无参构造函数

#### Declaration

```text
public UpdateHdataDefArgsV2()
```

### UpdateHdataDefArgsV2\(IList, String\) <a id="FBoxClientDriver_Contract_UpdateHdataDefArgsV2__ctor_System_Collections_Generic_IList_FBoxClientDriver_Contract_UpdateHdataDefinitionV2__System_String_"></a>

构造函数

#### Declaration

```text
public UpdateHdataDefArgsV2(IList updateHdatas, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IList&lt;[UpdateHdataDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataDefinitionV2.html)&gt; | updateHdatas | 更新的历史条目列表 |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_UpdateHdataDefArgsV2_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### UpdateHdatas <a id="FBoxClientDriver_Contract_UpdateHdataDefArgsV2_UpdateHdatas"></a>

#### Declaration

```text
public IList UpdateHdatas { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[UpdateHdataDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataDefinitionV2.html)&gt; |  |

