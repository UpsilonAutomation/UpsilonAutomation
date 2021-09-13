# PlcEntity

PLC 实体

#### Inheritance

System.Object

PlcEntity

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

#### Syntax <a id="FBoxClientDriver_Contract_PlcEntity_syntax"></a>

## Constructors <a id="constructors"></a>

### PlcEntity\(\) <a id="FBoxClientDriver_Contract_PlcEntity__ctor"></a>

构造函数

#### Declaration

## Properties <a id="properties"></a>

### ComPortPlcs <a id="FBoxClientDriver_Contract_PlcEntity_ComPortPlcs"></a>

串口PLC集合

#### Declaration

```text
public IList ComPortPlcs { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[ComPortPlc](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ComPortPlc.html)&gt; |  |

### EthernetPlcs <a id="FBoxClientDriver_Contract_PlcEntity_EthernetPlcs"></a>

网络PLC集合

#### Declaration

```text
public IList EthernetPlcs { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[EthernetPlc](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.EthernetPlc.html)&gt; |  |

