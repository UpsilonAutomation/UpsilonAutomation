# UpdateAlarmDefArgsV2

更新报警条目参数

#### Inheritance

System.Object

UpdateAlarmDefArgsV2

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateAlarmDefArgsV2_syntax"></a>

```text
public class UpdateAlarmDefArgsV2
```

## Constructors <a id="constructors"></a>

### UpdateAlarmDefArgsV2\(\) <a id="FBoxClientDriver_Contract_UpdateAlarmDefArgsV2__ctor"></a>

构造函数

#### Declaration

```text
public UpdateAlarmDefArgsV2()
```

### UpdateAlarmDefArgsV2\(IList, String\) <a id="FBoxClientDriver_Contract_UpdateAlarmDefArgsV2__ctor_System_Collections_Generic_IList_FBoxClientDriver_Contract_UpdateAlarmDefinitionV2__System_String_"></a>

构造函数

#### Declaration

```text
public UpdateAlarmDefArgsV2(IList updateAlarms, string boxNo)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IList&lt;[UpdateAlarmDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateAlarmDefinitionV2.html)&gt; | updateAlarms | 报警条目列表 [UpdateAlarmDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateAlarmDefinitionV2.html) |
| System.String | boxNo | 盒子编码 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_UpdateAlarmDefArgsV2_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### UpdateAlarms <a id="FBoxClientDriver_Contract_UpdateAlarmDefArgsV2_UpdateAlarms"></a>

#### Declaration

```text
public IList UpdateAlarms { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[UpdateAlarmDefinitionV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateAlarmDefinitionV2.html)&gt; |  |

