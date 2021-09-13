# AlarmDefinitionDtoV2

报警条目基类V2

#### Inheritance

System.Object

AlarmDefinitionDtoV2

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

#### Syntax <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_syntax"></a>

```text
public class AlarmDefinitionDtoV2 : DataSourceDtoV2
```

## Properties <a id="properties"></a>

### AlarmMessage <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_AlarmMessage"></a>

报警消息

#### Declaration

```text
[JsonProperty("alarmMsg")]
public string AlarmMessage { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Condition1 <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_Condition1"></a>

条件一，若选择bit数据类型，bit为ON:条件一EQ

#### Declaration

```text
[JsonProperty("condition1")]
public AlarmConditionType Condition1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |  |

### Condition2 <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_Condition2"></a>

报警条件二

#### Declaration

```text
[JsonProperty("condition2")]
public AlarmConditionType Condition2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |  |

### ConditionCombineMethod <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_ConditionCombineMethod"></a>

#### Declaration

```text
[JsonProperty("condMethod")]
public AlarmConditionCombineMethod ConditionCombineMethod { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |  |

### GroupId <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_GroupId"></a>

报警组别ID、报警组别名称使用一个即可

#### Declaration

```text
[JsonProperty("alarmGrpId")]
public long GroupId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### GroupName <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_GroupName"></a>

报警组别ID、报警组别名称使用一个即可

#### Declaration

```text
[JsonProperty("alarmGrpName")]
public string GroupName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Memo <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_Memo"></a>

报警备注

#### Declaration

```text
[JsonProperty("memo")]
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_Name"></a>

#### Declaration

```text
[JsonProperty("name")]
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Operand1 <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_Operand1"></a>

操作数一,若DataType为Bit\(位\)时,操作数一为0（OFF）或者1 \(ON\)

#### Declaration

```text
[JsonProperty("operand1")]
public decimal Operand1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Decimal |  |

### Operand2 <a id="FBoxClientDriver_Contract_AlarmDefinitionDtoV2_Operand2"></a>

操作数二,若DataType为Bit\(位\)时,操作数二为0， 若ConditionCombineMethod 为None时,也为0

#### Declaration

```text
[JsonProperty("operand2")]
public decimal Operand2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Decimal |  |

