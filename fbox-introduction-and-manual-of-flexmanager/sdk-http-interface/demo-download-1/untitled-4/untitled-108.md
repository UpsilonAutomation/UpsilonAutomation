# DownLoadPlcArgs

下载PLC参数

#### Inheritance

System.Object

System.EventArgs

DownLoadPlcArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_DownLoadPlcArgs_syntax"></a>

```text
public class DownLoadPlcArgs : EventArgs
```

## Constructors <a id="constructors"></a>

### DownLoadPlcArgs\(\) <a id="FBoxClientDriver_Contract_DownLoadPlcArgs__ctor"></a>

构造函数

#### Declaration

### DownLoadPlcArgs\(String, IDictionary, IList\) <a id="FBoxClientDriver_Contract_DownLoadPlcArgs__ctor_System_String_System_Collections_Generic_IDictionary_System_Int32_FBoxClientDriver_Contract_ComPortPlc__System_Collections_Generic_IList_FBoxClientDriver_Contract_EthernetPlc__"></a>

构造函数

#### Declaration

```text
public DownLoadPlcArgs(string boxNo, IDictionary comPortPlcs, IList ethernetPlcs)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Collections.Generic.IDictionary&lt;System.Int32, [ComPortPlc](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ComPortPlc.html)&gt; | comPortPlcs | 待下载串口PLC列表 |
| System.Collections.Generic.IList&lt;[EthernetPlc](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EthernetPlc.html)&gt; | ethernetPlcs | 待下载以太网PLC列表 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_DownLoadPlcArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### ComPortPlcs <a id="FBoxClientDriver_Contract_DownLoadPlcArgs_ComPortPlcs"></a>

待下载串口列表（目前仅支持 COM1,COM2,COM3） ,key=0代表com1 ,key=1代表com2,key=2代表com3

#### Declaration

```text
public IDictionary ComPortPlcs { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IDictionary&lt;System.Int32, [ComPortPlc](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ComPortPlc.html)&gt; |  |

### EthernetPlcs <a id="FBoxClientDriver_Contract_DownLoadPlcArgs_EthernetPlcs"></a>

待下载以太网PLC列表

#### Declaration

```text
public IList EthernetPlcs { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[EthernetPlc](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EthernetPlc.html)&gt; |  |

