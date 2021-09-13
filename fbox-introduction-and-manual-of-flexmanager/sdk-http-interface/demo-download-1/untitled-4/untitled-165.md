# UpdateDmonArgsV2

更新实时数据条目参数

#### Inheritance

System.Object

UpdateDmonArgsV2

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateDmonArgsV2_syntax"></a>

```text
public class UpdateDmonArgsV2
```

## Constructors <a id="constructors"></a>

### UpdateDmonArgsV2\(\) <a id="FBoxClientDriver_Contract_UpdateDmonArgsV2__ctor"></a>

构造函数

#### Declaration

```text
public UpdateDmonArgsV2()
```

### UpdateDmonArgsV2\(IList, String\) <a id="FBoxClientDriver_Contract_UpdateDmonArgsV2__ctor_System_Collections_Generic_IList_FBoxClientDriver_Contract_UpdateDataMonitorDefinitionV2__System_String_"></a>

构造函数

#### Declaration

```text
public UpdateDmonArgsV2(IList updateDmonList, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IList&lt;[UpdateDataMonitorDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateDataMonitorDefinitionV2.html)&gt; | updateDmonList | 更新的实时数据条目列表 |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_UpdateDmonArgsV2_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### UpdateDmonList <a id="FBoxClientDriver_Contract_UpdateDmonArgsV2_UpdateDmonList"></a>

#### Declaration

```text
public IList UpdateDmonList { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[UpdateDataMonitorDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateDataMonitorDefinitionV2.html)&gt; |  |

