# SignalRMessageArgs

SignalR信息参数

#### Inheritance

System.Object

System.EventArgs

SignalRMessageArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_SignalRMessageArgs_syntax"></a>

```text
public class SignalRMessageArgs : EventArgs
```

## Constructors <a id="constructors"></a>

### SignalRMessageArgs\(String, String, String, String\) <a id="FBoxClientDriver_Contract_SignalRMessageArgs__ctor_System_String_System_String_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public SignalRMessageArgs(string signalRUrl, string signalRId, string oldStatue, string newStatue)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | signalRUrl | SignalR地址 |
| System.String | signalRId | SignalR的ConnectId |
| System.String | oldStatue | 原先状态 |
| System.String | newStatue | 新状态 |

## Properties <a id="properties"></a>

### NewStatue <a id="FBoxClientDriver_Contract_SignalRMessageArgs_NewStatue"></a>

新状态

#### Declaration

```text
public string NewStatue { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### OldStatue <a id="FBoxClientDriver_Contract_SignalRMessageArgs_OldStatue"></a>

老状态

#### Declaration

```text
public string OldStatue { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### SignalRId <a id="FBoxClientDriver_Contract_SignalRMessageArgs_SignalRId"></a>

Url

#### Declaration

```text
public string SignalRId { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### SignalRUrl <a id="FBoxClientDriver_Contract_SignalRMessageArgs_SignalRUrl"></a>

地址

#### Declaration

```text
public string SignalRUrl { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

