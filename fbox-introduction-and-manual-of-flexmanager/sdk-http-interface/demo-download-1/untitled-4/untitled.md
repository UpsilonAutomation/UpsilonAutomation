# Box Information

盒子信息

#### Inheritance

System.Object

Box

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

#### Syntax <a id="FBoxClientDriver_Contract_Box_syntax"></a>

## Properties <a id="properties"></a>

### Alias <a id="FBoxClientDriver_Contract_Box_Alias"></a>

盒子名称

#### Declaration

```text
public string Alias { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### ApiBaseUrl <a id="FBoxClientDriver_Contract_Box_ApiBaseUrl"></a>

#### Declaration

```text
[JsonProperty("apiBaseUrl")]
public string ApiBaseUrl { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxNo <a id="FBoxClientDriver_Contract_Box_BoxNo"></a>

盒子编号

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxType <a id="FBoxClientDriver_Contract_Box_BoxType"></a>

盒子类型

#### Declaration

```text
public BoxTypes BoxType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxTypes.html) |  |

### ConnectionState <a id="FBoxClientDriver_Contract_Box_ConnectionState"></a>

盒子状态

#### Declaration

```text
public BoxConnectionState ConnectionState { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) |  |

### Disabled <a id="FBoxClientDriver_Contract_Box_Disabled"></a>

#### Declaration

```text
[JsonProperty("disabled")]
public bool Disabled { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### NetworkType <a id="FBoxClientDriver_Contract_Box_NetworkType"></a>

当前网络类型

#### Declaration

```text
[JsonProperty("net")]
public NetworkTypes NetworkType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [NetworkTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.NetworkTypes.html) |  |

### Owned <a id="FBoxClientDriver_Contract_Box_Owned"></a>

#### Declaration

```text
public bool Owned { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### SignalrUrl <a id="FBoxClientDriver_Contract_Box_SignalrUrl"></a>

#### Declaration

```text
[JsonProperty("signalrUrl")]
public string SignalrUrl { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

