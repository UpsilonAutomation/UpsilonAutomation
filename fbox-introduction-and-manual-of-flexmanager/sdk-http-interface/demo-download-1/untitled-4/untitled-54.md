# ComPortPlc

串口参数

#### Inheritance

System.Object

ComPortPlc

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

#### Syntax <a id="FBoxClientDriver_Contract_ComPortPlc_syntax"></a>

```text
public class ComPortPlc : BasePlcParameter
```

## Properties <a id="properties"></a>

### BaudRate <a id="FBoxClientDriver_Contract_ComPortPlc_BaudRate"></a>

波特率

#### Declaration

```text
public int BaudRate { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### DataBits <a id="FBoxClientDriver_Contract_ComPortPlc_DataBits"></a>

数据位

#### Declaration

```text
public int DataBits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Parity <a id="FBoxClientDriver_Contract_ComPortPlc_Parity"></a>

校验位

#### Declaration

```text
public ParityType Parity { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [ParityType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ParityType.html) |  |

### StopBits <a id="FBoxClientDriver_Contract_ComPortPlc_StopBits"></a>

停止位

#### Declaration

```text
public int StopBits { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### WorkingModel <a id="FBoxClientDriver_Contract_ComPortPlc_WorkingModel"></a>

#### Declaration

```text
public WorkModel WorkingModel { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [WorkModel](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.WorkModel.html) |  |

