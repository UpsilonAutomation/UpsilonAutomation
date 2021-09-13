# AddOrUpdateCombinedItemArgs.DMonItemArgsV2

#### Inheritance

System.Object

AddOrUpdateCombinedItemArgs.DMonItemArgsV2

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

#### Syntax <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_syntax"></a>

```text
public class DMonItemArgsV2
```

## Properties <a id="properties"></a>

### BitStateLabel <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_BitStateLabel"></a>

#### Declaration

```text
[JsonProperty("label")]
public BitStateLabel BitStateLabel { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BitStateLabel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BitStateLabel.html) |  |

### CharCount <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_CharCount"></a>

#### Declaration

```text
public int CharCount { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DataType <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_DataType"></a>

#### Declaration

```text
public DataType DataType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### DeadValue <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_DeadValue"></a>

#### Declaration

```text
public float DeadValue { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Single |  |

### Encoding <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_Encoding"></a>

#### Declaration

```text
public EncodeType Encoding { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [EncodeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EncodeType.html) |  |

### FractionalDigits <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_FractionalDigits"></a>

#### Declaration

```text
[JsonProperty("fracDigits")]
public int FractionalDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### GroupId <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_GroupId"></a>

#### Declaration

```text
[JsonProperty("dmonGrpId")]
public long GroupId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### GroupName <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_GroupName"></a>

#### Declaration

```text
[JsonProperty("dmonGrpName")]
public string GroupName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Id <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_Id"></a>

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### IntegralDigits <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_IntegralDigits"></a>

#### Declaration

```text
[JsonProperty("intDigits")]
public int IntegralDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IoWidth <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_IoWidth"></a>

#### Declaration

```text
public DataWidth IoWidth { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |  |

### IsDeviceChanged <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_IsDeviceChanged"></a>

#### Declaration

```text
[JsonIgnore]
[JsonProperty("deviceChanged")]
public bool IsDeviceChanged { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### MainAddress <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_MainAddress"></a>

#### Declaration

```text
[JsonProperty("addr")]
public int MainAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Memo <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_Memo"></a>

#### Declaration

```text
[JsonProperty("memo")]
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_Name"></a>

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### PlcName <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_PlcName"></a>

#### Declaration

```text
[JsonProperty("devAlias")]
public string PlcName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Privilege <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_Privilege"></a>

#### Declaration

```text
[JsonProperty("privilege")]
public PrivilegeType Privilege { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) |  |

### RegId <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_RegId"></a>

#### Declaration

```text
public int RegId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegName <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_RegName"></a>

#### Declaration

```text
[JsonProperty("regName")]
public string RegName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### StationNo <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_StationNo"></a>

#### Declaration

```text
[JsonProperty("station")]
public int StationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StringByteOrder <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_StringByteOrder"></a>

#### Declaration

```text
public StringByteOrder StringByteOrder { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [StringByteOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StringByteOrder.html) |  |

### SubAddress <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_SubAddress"></a>

#### Declaration

```text
[JsonProperty("subAddr")]
public int SubAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubIndex <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_SubIndex"></a>

#### Declaration

```text
[JsonProperty("addrBlk")]
public int SubIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### TaskState <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_TaskState"></a>

#### Declaration

```text
[JsonProperty("tstate")]
public int TaskState { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### TrafficSaving <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_TrafficSaving"></a>

#### Declaration

```text
[JsonProperty("trafficSaving")]
public bool TrafficSaving { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Unit <a id="FBoxClientDriver_Contract_AddOrUpdateCombinedItemArgs_DMonItemArgsV2_Unit"></a>

#### Declaration

```text
public string Unit { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

