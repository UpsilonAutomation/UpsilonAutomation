# BoxLocationEventArgs

SignalR推送的地址位置

#### Inheritance

System.Object

System.EventArgs

BoxLocationEventArgs

#### Inherited Members

System.EventArgs.Empty

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver.SignalREventArgs**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_SignalREventArgs_BoxLocationEventArgs_syntax"></a>

```text
public class BoxLocationEventArgs : EventArgs
```

## Constructors <a id="constructors"></a>

### BoxLocationEventArgs\(Int64, String, Double, Double, Int32, String\) <a id="FBoxClientDriver_SignalREventArgs_BoxLocationEventArgs__ctor_System_Int64_System_String_System_Double_System_Double_System_Int32_System_String_"></a>

构造函数

#### Declaration

```text
public BoxLocationEventArgs(long boxId, string boxNo, double latitude, double longitude, int radius, string address)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | boxId |  |
| System.String | boxNo |  |
| System.Double | latitude |  |
| System.Double | longitude |  |
| System.Int32 | radius |  |
| System.String | address |  |

## Properties <a id="properties"></a>

### Address <a id="FBoxClientDriver_SignalREventArgs_BoxLocationEventArgs_Address"></a>

#### Declaration

```text
public string Address { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxId <a id="FBoxClientDriver_SignalREventArgs_BoxLocationEventArgs_BoxId"></a>

#### Declaration

```text
public long BoxId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### BoxNo <a id="FBoxClientDriver_SignalREventArgs_BoxLocationEventArgs_BoxNo"></a>

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Latitude <a id="FBoxClientDriver_SignalREventArgs_BoxLocationEventArgs_Latitude"></a>

#### Declaration

```text
public double Latitude { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Double |  |

### Longitude <a id="FBoxClientDriver_SignalREventArgs_BoxLocationEventArgs_Longitude"></a>

#### Declaration

```text
public double Longitude { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Double |  |

### Radius <a id="FBoxClientDriver_SignalREventArgs_BoxLocationEventArgs_Radius"></a>

#### Declaration

```text
public int Radius { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

