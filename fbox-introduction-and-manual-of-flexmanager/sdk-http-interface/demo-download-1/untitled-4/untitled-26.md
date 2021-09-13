# AlarmDefintitionDtoV2

报警条目V2

#### Inheritance

System.Object

AlarmDefintitionDtoV2

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

#### Syntax <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_syntax"></a>

```text
public class AlarmDefintitionDtoV2 : DataSourceDtoV2
```

## Properties <a id="properties"></a>

### AlarmGroup <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_AlarmGroup"></a>

#### Declaration

```text
[JsonProperty("group")]
public AlarmGroupDtoV2 AlarmGroup { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmGroupDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmGroupDtoV2.html) |  |

### AlarmMessage <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_AlarmMessage"></a>

报警信息

#### Declaration

```text
[JsonProperty("alarmMsg")]
public string AlarmMessage { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Code <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_Code"></a>

报警条目编码

#### Declaration

```text
public int Code { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Condition1 <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_Condition1"></a>

#### Declaration

```text
public AlarmConditionType Condition1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |  |

### Condition2 <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_Condition2"></a>

#### Declaration

```text
public AlarmConditionType Condition2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionType.html) |  |

### ConditionCombineMethod <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_ConditionCombineMethod"></a>

#### Declaration

```text
[JsonProperty("condMethod")]
public AlarmConditionCombineMethod ConditionCombineMethod { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmConditionCombineMethod](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConditionCombineMethod.html) |  |

### Id <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_Id"></a>

报警条目Id

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### IsDeviceChanged <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_IsDeviceChanged"></a>

设备是否已经变更

#### Declaration

```text
[JsonProperty("deviceChanged")]
public bool IsDeviceChanged { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Memo <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_Memo"></a>

备注

#### Declaration

```text
[JsonProperty("memo")]
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_Name"></a>

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Operand1 <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_Operand1"></a>

操作数一

#### Declaration

```text
public decimal Operand1 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Decimal |  |

### Operand2 <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_Operand2"></a>

操作数二

#### Declaration

```text
public decimal Operand2 { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Decimal |  |

### TaskState <a id="FBoxClientDriver_Contract_AlarmDefintitionDtoV2_TaskState"></a>

#### Declaration

```text
[JsonProperty("tstate")]
public TaskState TaskState { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [TaskState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.TaskState.html) |  |

