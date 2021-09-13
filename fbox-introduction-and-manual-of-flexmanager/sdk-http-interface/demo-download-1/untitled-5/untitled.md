# BoxConnectionStateItem

盒子状态

#### Inheritance

System.Object

System.EventArgs

BoxConnectionStateItem

#### Inherited Members

System.EventArgs.Empty

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_BoxConnectionStateItem_syntax"></a>

```text
public class BoxConnectionStateItem : EventArgs
```

## Properties <a id="properties"></a>

### AlarmCount <a id="FBoxClientDriver_BoxConnectionStateItem_AlarmCount"></a>

#### Declaration

```text
[JsonProperty("alarmCount")]
public int AlarmCount { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### BoxNo <a id="FBoxClientDriver_BoxConnectionStateItem_BoxNo"></a>

#### Declaration

```text
[JsonProperty("boxNo")]
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxTaskState <a id="FBoxClientDriver_BoxConnectionStateItem_BoxTaskState"></a>

#### Declaration

```text
[JsonProperty("tstate")]
public BoxTaskState BoxTaskState { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxTaskState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.BoxTaskState.html) |  |

### BoxUid <a id="FBoxClientDriver_BoxConnectionStateItem_BoxUid"></a>

#### Declaration

```text
[JsonProperty("id")]
public long BoxUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Features <a id="FBoxClientDriver_BoxConnectionStateItem_Features"></a>

#### Declaration

```text
[JsonProperty("feat")]
public BoxFeatures Features { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxFeatures](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.BoxFeatures.html) |  |

### NetworkType <a id="FBoxClientDriver_BoxConnectionStateItem_NetworkType"></a>

#### Declaration

```text
[JsonProperty("net")]
public NetworkTypes NetworkType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [NetworkTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.NetworkTypes.html) |  |

### NewState <a id="FBoxClientDriver_BoxConnectionStateItem_NewState"></a>

#### Declaration

```text
[JsonProperty("state")]
public BoxConnectionState NewState { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) |  |

### OperationMode <a id="FBoxClientDriver_BoxConnectionStateItem_OperationMode"></a>

#### Declaration

```text
[JsonProperty("mode")]
public BoxOperationMode OperationMode { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxOperationMode](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.BoxOperationMode.html) |  |

#### Declaration

```text
[JsonProperty("rssi")]
public int Rssi { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SoftwareVersions <a id="FBoxClientDriver_BoxConnectionStateItem_SoftwareVersions"></a>

#### Declaration

```text
[JsonProperty("vers")]
public IDictionary SoftwareVersions { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IDictionary&lt;[BoxSoftwareTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.BoxSoftwareTypes.html), System.Int32&gt; |  |

### TimeZoneString <a id="FBoxClientDriver_BoxConnectionStateItem_TimeZoneString"></a>

#### Declaration

```text
[JsonProperty("tz")]
public string TimeZoneString { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

