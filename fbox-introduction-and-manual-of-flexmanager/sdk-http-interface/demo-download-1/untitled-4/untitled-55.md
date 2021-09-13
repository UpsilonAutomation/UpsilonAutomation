# DataMonitorDefinition

数据监控点

#### Inheritance

System.Object

DataMonitorDefinition

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

#### Syntax <a id="FBoxClientDriver_Contract_DataMonitorDefinition_syntax"></a>

```text
public class DataMonitorDefinition
```

## Properties <a id="properties"></a>

### DataType <a id="FBoxClientDriver_Contract_DataMonitorDefinition_DataType"></a>

监控点数据类型

#### Declaration

```text
public DataType DataType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) |  |

### Description <a id="FBoxClientDriver_Contract_DataMonitorDefinition_Description"></a>

监控点条目描述

#### Declaration

```text
public string Description { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### DeviceId <a id="FBoxClientDriver_Contract_DataMonitorDefinition_DeviceId"></a>

设备ID

#### Declaration

```text
public int DeviceId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DMonGroupUid <a id="FBoxClientDriver_Contract_DataMonitorDefinition_DMonGroupUid"></a>

分组

#### Declaration

```text
public long DMonGroupUid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### FractionalDigits <a id="FBoxClientDriver_Contract_DataMonitorDefinition_FractionalDigits"></a>

小数位

#### Declaration

```text
public int FractionalDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IntegralDigits <a id="FBoxClientDriver_Contract_DataMonitorDefinition_IntegralDigits"></a>

整数位

#### Declaration

```text
public int IntegralDigits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IP <a id="FBoxClientDriver_Contract_DataMonitorDefinition_IP"></a>

IP地址

#### Declaration

```text
public string IP { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### MainAddress <a id="FBoxClientDriver_Contract_DataMonitorDefinition_MainAddress"></a>

主地址

#### Declaration

```text
public int MainAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Name <a id="FBoxClientDriver_Contract_DataMonitorDefinition_Name"></a>

监控点条目名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Port <a id="FBoxClientDriver_Contract_DataMonitorDefinition_Port"></a>

端口号

#### Declaration

```text
public int Port { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### PortNo <a id="FBoxClientDriver_Contract_DataMonitorDefinition_PortNo"></a>

portNo

#### Declaration

```text
public int PortNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Privilege <a id="FBoxClientDriver_Contract_DataMonitorDefinition_Privilege"></a>

读写权限

#### Declaration

```text
public PrivilegeType Privilege { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [PrivilegeType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PrivilegeType.html) |  |

### RegisterId <a id="FBoxClientDriver_Contract_DataMonitorDefinition_RegisterId"></a>

寄存器ID

#### Declaration

```text
public int RegisterId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### RegisterWidth <a id="FBoxClientDriver_Contract_DataMonitorDefinition_RegisterWidth"></a>

数据宽度类型

#### Declaration

```text
public DataWidth RegisterWidth { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |  |

### ServerId <a id="FBoxClientDriver_Contract_DataMonitorDefinition_ServerId"></a>

服务ID

#### Declaration

```text
public int ServerId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### StationNo <a id="FBoxClientDriver_Contract_DataMonitorDefinition_StationNo"></a>

站号

#### Declaration

```text
public int StationNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubAddress <a id="FBoxClientDriver_Contract_DataMonitorDefinition_SubAddress"></a>

子地址

#### Declaration

```text
public int SubAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubIndex <a id="FBoxClientDriver_Contract_DataMonitorDefinition_SubIndex"></a>

西门子DB块地址

#### Declaration

```text
public int SubIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Uid <a id="FBoxClientDriver_Contract_DataMonitorDefinition_Uid"></a>

数据监控条目UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Unit <a id="FBoxClientDriver_Contract_DataMonitorDefinition_Unit"></a>

单位

#### Declaration

```text
public string Unit { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### UpdateInterval <a id="FBoxClientDriver_Contract_DataMonitorDefinition_UpdateInterval"></a>

更新频率

#### Declaration

```text
public int UpdateInterval { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### ZeroPaddingLeft <a id="FBoxClientDriver_Contract_DataMonitorDefinition_ZeroPaddingLeft"></a>

前置0

#### Declaration

```text
public bool ZeroPaddingLeft { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### ZeroPaddingRight <a id="FBoxClientDriver_Contract_DataMonitorDefinition_ZeroPaddingRight"></a>

后置0

#### Declaration

```text
public bool ZeroPaddingRight { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

