# RegisterInfo

寄存器信息

#### Inheritance

System.Object

RegisterInfo

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

#### Syntax <a id="FBoxClientDriver_Contract_RegisterInfo_syntax"></a>

```text
public class RegisterInfo
```

## Properties <a id="properties"></a>

### Id <a id="FBoxClientDriver_Contract_RegisterInfo_Id"></a>

寄存器ID 对于同一个设备，此值不唯一，需要和[IoWidth]()联合方可确定一个寄存器

#### Declaration

```text
public int Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### IoWidth <a id="FBoxClientDriver_Contract_RegisterInfo_IoWidth"></a>

数据宽度类型

#### Declaration

```text
public DataWidth IoWidth { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |  |

### IsBigEndian <a id="FBoxClientDriver_Contract_RegisterInfo_IsBigEndian"></a>

是否大端

#### Declaration

```text
public bool IsBigEndian { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### MainAddressType <a id="FBoxClientDriver_Contract_RegisterInfo_MainAddressType"></a>

主地址进制类型

#### Declaration

```text
public AddressRadixType MainAddressType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AddressRadixType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddressRadixType.html) |  |

### MainAddressWidth <a id="FBoxClientDriver_Contract_RegisterInfo_MainAddressWidth"></a>

主地址寻址方式

#### Declaration

```text
public DataWidth MainAddressWidth { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) |  |

### MaxMainAddress <a id="FBoxClientDriver_Contract_RegisterInfo_MaxMainAddress"></a>

主地址寻址上限

#### Declaration

```text
public int MaxMainAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MaxSubIndex <a id="FBoxClientDriver_Contract_RegisterInfo_MaxSubIndex"></a>

最大索引地址

#### Declaration

```text
public int MaxSubIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MinMainAddress <a id="FBoxClientDriver_Contract_RegisterInfo_MinMainAddress"></a>

主地址寻址下限

#### Declaration

```text
public int MinMainAddress { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### MinSubIndex <a id="FBoxClientDriver_Contract_RegisterInfo_MinSubIndex"></a>

子地址索引最小值

#### Declaration

```text
public int MinSubIndex { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### Name <a id="FBoxClientDriver_Contract_RegisterInfo_Name"></a>

寄存器名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### SubAddressLength <a id="FBoxClientDriver_Contract_RegisterInfo_SubAddressLength"></a>

子地址长度

#### Declaration

```text
public int SubAddressLength { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

### SubAddressType <a id="FBoxClientDriver_Contract_RegisterInfo_SubAddressType"></a>

子地址进制类型

#### Declaration

```text
public AddressRadixType SubAddressType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AddressRadixType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddressRadixType.html) |  |

### SubIndexType <a id="FBoxClientDriver_Contract_RegisterInfo_SubIndexType"></a>

西门子DB块地址进制类型

#### Declaration

```text
public AddressRadixType SubIndexType { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| [AddressRadixType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddressRadixType.html) |  |

