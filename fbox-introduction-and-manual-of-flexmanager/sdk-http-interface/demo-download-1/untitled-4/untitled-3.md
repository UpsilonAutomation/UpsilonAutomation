# AlarmTriggerDefinitionArgs

报警条目触发参数

#### Inheritance

System.Object

System.EventArgs

AlarmTriggerDefinitionArgs

#### Inherited Members

System.EventArgs.Empty

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver.Contract**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_AlarmTriggerDefinitionArgs_syntax"></a>

```text
public class AlarmTriggerDefinitionArgs : EventArgs
```

## Properties <a id="properties"></a>

### BoxId <a id="FBoxClientDriver_Contract_AlarmTriggerDefinitionArgs_BoxId"></a>

盒子Id

#### Declaration

```text
public long BoxId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### BoxNo <a id="FBoxClientDriver_Contract_AlarmTriggerDefinitionArgs_BoxNo"></a>

报警盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Message <a id="FBoxClientDriver_Contract_AlarmTriggerDefinitionArgs_Message"></a>

报警内容

#### Declaration

```text
public string Message { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_AlarmTriggerDefinitionArgs_Name"></a>

报警名称\[暂时为报警编码代替\]

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Status <a id="FBoxClientDriver_Contract_AlarmTriggerDefinitionArgs_Status"></a>

状态

#### Declaration

```text
public DMonStatus Status { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DMonStatus](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DMonStatus.html) |  |

### Uid <a id="FBoxClientDriver_Contract_AlarmTriggerDefinitionArgs_Uid"></a>

报警条目的UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Value <a id="FBoxClientDriver_Contract_AlarmTriggerDefinitionArgs_Value"></a>

报警条目的值

#### Declaration

```text
public object Value { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Object |  |

