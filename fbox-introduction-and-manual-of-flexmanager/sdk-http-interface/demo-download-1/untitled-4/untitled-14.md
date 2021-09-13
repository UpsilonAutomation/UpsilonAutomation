# AddDmonsArgsV2

新增监控点参数

#### Inheritance

System.Object

AddDmonsArgsV2

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

#### Syntax <a id="FBoxClientDriver_Contract_AddDmonsArgsV2_syntax"></a>

```text
public class AddDmonsArgsV2
```

## Constructors <a id="constructors"></a>

### AddDmonsArgsV2\(\) <a id="FBoxClientDriver_Contract_AddDmonsArgsV2__ctor"></a>

构造函数

#### Declaration

### AddDmonsArgsV2\(IList, String\) <a id="FBoxClientDriver_Contract_AddDmonsArgsV2__ctor_System_Collections_Generic_IList_FBoxClientDriver_Contract_AddDataMonitorDefinitionV2__System_String_"></a>

构造函数

#### Declaration

```text
public AddDmonsArgsV2(IList addDmons, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IList&lt;[AddDataMonitorDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddDataMonitorDefinitionV2.html)&gt; | addDmons | 实时数据条目列表 |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### AddDmons <a id="FBoxClientDriver_Contract_AddDmonsArgsV2_AddDmons"></a>

#### Declaration

```text
public IList AddDmons { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[AddDataMonitorDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddDataMonitorDefinitionV2.html)&gt; |  |

### BoxNo <a id="FBoxClientDriver_Contract_AddDmonsArgsV2_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

