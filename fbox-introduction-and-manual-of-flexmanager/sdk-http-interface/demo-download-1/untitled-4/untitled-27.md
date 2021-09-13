# AlarmEvent

报警记录信息

#### Inheritance

System.Object

AlarmEvent

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

#### Syntax <a id="FBoxClientDriver_Contract_AlarmEvent_syntax"></a>

## Properties <a id="properties"></a>

### Action <a id="FBoxClientDriver_Contract_AlarmEvent_Action"></a>

#### Declaration

```text
[JsonProperty("a")]
public AlarmAction Action { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AlarmAction](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmAction.html) |  |

### AlarmId <a id="FBoxClientDriver_Contract_AlarmEvent_AlarmId"></a>

报警条目UID

#### Declaration

```text
[JsonProperty("i")]
public long AlarmId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Code <a id="FBoxClientDriver_Contract_AlarmEvent_Code"></a>

报警条目（编码）

#### Declaration

```text
[JsonProperty("n")]
public string Code { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Message <a id="FBoxClientDriver_Contract_AlarmEvent_Message"></a>

报警内容

#### Declaration

```text
[JsonProperty("m")]
public string Message { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_AlarmEvent_Name"></a>

报警名称

#### Declaration

```text
[JsonProperty("rn")]
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Timestamp <a id="FBoxClientDriver_Contract_AlarmEvent_Timestamp"></a>

报警触发时间

#### Declaration

```text
[JsonIgnore]
public DateTime Timestamp { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### TimestampUnixEpoch <a id="FBoxClientDriver_Contract_AlarmEvent_TimestampUnixEpoch"></a>

UNIX时间戳

#### Declaration

```text
[JsonProperty("t")]
public long TimestampUnixEpoch { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Value <a id="FBoxClientDriver_Contract_AlarmEvent_Value"></a>

值

#### Declaration

```text
[JsonProperty("v")]
public object Value { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Object |  |

## Methods <a id="methods"></a>

### ShouldSerializeAlarmId\(\) <a id="FBoxClientDriver_Contract_AlarmEvent_ShouldSerializeAlarmId"></a>

是否显示报警条目Id

#### Declaration

```text
public bool ShouldSerializeAlarmId()
```

#### Returns

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

