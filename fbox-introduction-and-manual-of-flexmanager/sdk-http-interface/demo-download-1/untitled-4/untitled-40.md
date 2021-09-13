# BoxConnectionStateChangedEventArgs

盒子状态更新参数

#### Inheritance

System.Object

System.EventArgs

BoxConnectionStateChangedEventArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_BoxConnectionStateChangedEventArgs_syntax"></a>

```text
public class BoxConnectionStateChangedEventArgs : EventArgs
```

## Constructors <a id="constructors"></a>

### BoxConnectionStateChangedEventArgs\(String, BoxConnectionState, BoxConnectionState\) <a id="FBoxClientDriver_Contract_BoxConnectionStateChangedEventArgs__ctor_System_String_FBoxClientDriver_Contract_BoxConnectionState_FBoxClientDriver_Contract_BoxConnectionState_"></a>

Constructor

#### Declaration

```text
public BoxConnectionStateChangedEventArgs(string boxNo, BoxConnectionState oldState, BoxConnectionState newState)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) | oldState | 老的状态 |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) | newState | 新的状态 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_BoxConnectionStateChangedEventArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### NewState <a id="FBoxClientDriver_Contract_BoxConnectionStateChangedEventArgs_NewState"></a>

新状态

#### Declaration

```text
public BoxConnectionState NewState { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) |  |

### OldState <a id="FBoxClientDriver_Contract_BoxConnectionStateChangedEventArgs_OldState"></a>

老状态

#### Declaration

```text
public BoxConnectionState OldState { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [BoxConnectionState](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxConnectionState.html) |  |

