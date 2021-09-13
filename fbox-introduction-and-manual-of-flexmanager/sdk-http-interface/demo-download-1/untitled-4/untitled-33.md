# AlarmRecoverDefinitonArgs

报警条目还原参数

#### Inheritance

System.Object

System.EventArgs

AlarmRecoverDefinitonArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_AlarmRecoverDefinitonArgs_syntax"></a>

```text
public class AlarmRecoverDefinitonArgs : EventArgs
```

## Properties <a id="properties"></a>

### BoxId <a id="FBoxClientDriver_Contract_AlarmRecoverDefinitonArgs_BoxId"></a>

盒子ID

#### Declaration

```text
public long BoxId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### BoxNo <a id="FBoxClientDriver_Contract_AlarmRecoverDefinitonArgs_BoxNo"></a>

报警盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Message <a id="FBoxClientDriver_Contract_AlarmRecoverDefinitonArgs_Message"></a>

报警内容

#### Declaration

```text
public string Message { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_AlarmRecoverDefinitonArgs_Name"></a>

报警名称\[暂时为报警编码代替\]

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_AlarmRecoverDefinitonArgs_Uid"></a>

报警条目的UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Value <a id="FBoxClientDriver_Contract_AlarmRecoverDefinitonArgs_Value"></a>

报警条目的值

#### Declaration

```text
public object Value { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Object |  |

