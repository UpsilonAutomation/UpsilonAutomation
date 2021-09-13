# DMonDtoV2

监控点参数

#### Inheritance

System.Object

DMonDtoV2

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

#### Syntax <a id="FBoxClientDriver_Contract_DMonDtoV2_syntax"></a>

```text
public class DMonDtoV2 : DataSourceDtoV2
```

## Properties <a id="properties"></a>

### BitStateLabel <a id="FBoxClientDriver_Contract_DMonDtoV2_BitStateLabel"></a>

#### Declaration

```text
[JsonProperty("label")]
public BitStateLabel BitStateLabel { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BitStateLabel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BitStateLabel.html) |  |

### CharCount <a id="FBoxClientDriver_Contract_DMonDtoV2_CharCount"></a>

字符个数

#### Declaration

```text
public int CharCount { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DeadValue <a id="FBoxClientDriver_Contract_DMonDtoV2_DeadValue"></a>

死区值

#### Declaration

```text
public float DeadValue { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Single |  |

### Encoding <a id="FBoxClientDriver_Contract_DMonDtoV2_Encoding"></a>

#### Declaration

```text
public EncodeType Encoding { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [EncodeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EncodeType.html) |  |

### FractionalDigits <a id="FBoxClientDriver_Contract_DMonDtoV2_FractionalDigits"></a>

小数位

#### Declaration

```text
[JsonProperty("fracDigits")]
public int FractionalDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### GroupId <a id="FBoxClientDriver_Contract_DMonDtoV2_GroupId"></a>

监控点分组ID,和GroupName任选一个使用，优先级是名称

#### Declaration

```text
[JsonProperty("dmonGrpId")]
public long GroupId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### GroupName <a id="FBoxClientDriver_Contract_DMonDtoV2_GroupName"></a>

监控点分组名称，和GroupId任选一个使用，若使用不存在的监控点分组，则会自动新增该分组

#### Declaration

```text
[JsonProperty("dmonGrpName")]
public string GroupName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### IntegralDigits <a id="FBoxClientDriver_Contract_DMonDtoV2_IntegralDigits"></a>

整数位\(目前无作用\)

#### Declaration

```text
[JsonProperty("intDigits")]
public int IntegralDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Memo <a id="FBoxClientDriver_Contract_DMonDtoV2_Memo"></a>

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

### Name <a id="FBoxClientDriver_Contract_DMonDtoV2_Name"></a>

监控点名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Privilege <a id="FBoxClientDriver_Contract_DMonDtoV2_Privilege"></a>

#### Declaration

```text
[JsonProperty("privilege")]
public PrivilegeType Privilege { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) |  |

### StringByteOrder <a id="FBoxClientDriver_Contract_DMonDtoV2_StringByteOrder"></a>

#### Declaration

```text
public StringByteOrder StringByteOrder { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [StringByteOrder](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StringByteOrder.html) |  |

### TrafficSaving <a id="FBoxClientDriver_Contract_DMonDtoV2_TrafficSaving"></a>

省流量模式

#### Declaration

```text
[JsonProperty("trafficSaving")]
public bool TrafficSaving { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Unit <a id="FBoxClientDriver_Contract_DMonDtoV2_Unit"></a>

单位

#### Declaration

```text
public string Unit { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### ValueTransform <a id="FBoxClientDriver_Contract_DMonDtoV2_ValueTransform"></a>

数据运算

#### Declaration

```text
[JsonProperty("valueTransform")]
public DmonValueTransform ValueTransform { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DmonValueTransform](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DmonValueTransform.html) |  |

