# DataSourceDtoV2

数据源基类

#### Inheritance

System.Object

DataSourceDtoV2

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

#### Syntax <a id="FBoxClientDriver_Contract_DataSourceDtoV2_syntax"></a>

```text
public class DataSourceDtoV2
```

## Properties <a id="properties"></a>

### AddressDescription <a id="FBoxClientDriver_Contract_DataSourceDtoV2_AddressDescription"></a>

地址描述

#### Declaration

```text
[JsonProperty("addrDesc")]
public string AddressDescription { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BitIndex <a id="FBoxClientDriver_Contract_DataSourceDtoV2_BitIndex"></a>

按位索引号

#### Declaration

```text
public int BitIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### BitIndexEnabled <a id="FBoxClientDriver_Contract_DataSourceDtoV2_BitIndexEnabled"></a>

是否启用按位索引

#### Declaration

```text
public bool BitIndexEnabled { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### DataType <a id="FBoxClientDriver_Contract_DataSourceDtoV2_DataType"></a>

#### Declaration

```text
public DataType DataType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### DevAlias <a id="FBoxClientDriver_Contract_DataSourceDtoV2_DevAlias"></a>

PLC别名

#### Declaration

```text
[JsonProperty("devAlias")]
public string DevAlias { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### IoWidth <a id="FBoxClientDriver_Contract_DataSourceDtoV2_IoWidth"></a>

#### Declaration

```text
public DataWidth IoWidth { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |  |

### MainAddress <a id="FBoxClientDriver_Contract_DataSourceDtoV2_MainAddress"></a>

主地址

#### Declaration

```text
[JsonProperty("addr")]
public int MainAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegId <a id="FBoxClientDriver_Contract_DataSourceDtoV2_RegId"></a>

寄存器ID（与寄存器位宽联合使用）

#### Declaration

```text
public int RegId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegName <a id="FBoxClientDriver_Contract_DataSourceDtoV2_RegName"></a>

寄存器名称

#### Declaration

```text
[JsonProperty("regName")]
public string RegName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### StationNo <a id="FBoxClientDriver_Contract_DataSourceDtoV2_StationNo"></a>

站号

#### Declaration

```text
[JsonProperty("station")]
public int StationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubAddress <a id="FBoxClientDriver_Contract_DataSourceDtoV2_SubAddress"></a>

子地址

#### Declaration

```text
[JsonProperty("subAddr")]
public int SubAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubIndex <a id="FBoxClientDriver_Contract_DataSourceDtoV2_SubIndex"></a>

数据块\(DB块\)

#### Declaration

```text
[JsonProperty("addrBlk")]
public int SubIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

