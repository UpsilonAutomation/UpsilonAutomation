# AlarmMonitorDefinition

报警条目

#### Inheritance

System.Object

AlarmMonitorDefinition

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

#### Syntax <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_syntax"></a>

```text
public class AlarmMonitorDefinition
```

## Properties <a id="properties"></a>

### AlarmMessage <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_AlarmMessage"></a>

报警信息

#### Declaration

```text
public string AlarmMessage { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### AlarmState <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_AlarmState"></a>

报警状态

#### Declaration

```text
public AlarmState AlarmState { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmState.html) |  |

### Code <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_Code"></a>

报警编码

#### Declaration

```text
public int Code { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Condition1 <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_Condition1"></a>

条件一

#### Declaration

```text
public AlarmConditionType Condition1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |  |

### Condition2 <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_Condition2"></a>

条件二

#### Declaration

```text
public AlarmConditionType Condition2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |  |

### ConditionCombineMethod <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_ConditionCombineMethod"></a>

条件组合

#### Declaration

```text
[JsonProperty("condMethod")]
public AlarmConditionCombineMethod ConditionCombineMethod { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |  |

### LastRecoveredTime <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_LastRecoveredTime"></a>

最后恢复事件

#### Declaration

```text
public DateTime? LastRecoveredTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Nullable&lt;System.DateTime&gt; |  |

### LastTriggeredTime <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_LastTriggeredTime"></a>

最后触发时间

#### Declaration

```text
public DateTime? LastTriggeredTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Nullable&lt;System.DateTime&gt; |  |

### Memo <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_Memo"></a>

备注

#### Declaration

```text
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_Name"></a>

报警名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Operand1 <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_Operand1"></a>

操作数一

#### Declaration

```text
public decimal Operand1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Decimal |  |

### Operand2 <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_Operand2"></a>

操作数二

#### Declaration

```text
public decimal Operand2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Decimal |  |

### Uid <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_Uid"></a>

报警条目UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### ValueOnLastEvent <a id="FBoxClientDriver_Contract_AlarmMonitorDefinition_ValueOnLastEvent"></a>

最后的值

#### Declaration

```text
public object ValueOnLastEvent { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Object |  |

