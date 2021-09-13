# UpdateHdataChannelsDto

历史记录多通道更新对象

#### Inheritance

System.Object

UpdateHdataChannelsDto

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateHdataChannelsDto_syntax"></a>

```text
public class UpdateHdataChannelsDto : HdataChannelDto
```

## Constructors <a id="constructors"></a>

### UpdateHdataChannelsDto\(\) <a id="FBoxClientDriver_Contract_UpdateHdataChannelsDto__ctor"></a>

#### Declaration

```text
public UpdateHdataChannelsDto()
```

### UpdateHdataChannelsDto\(Int64, String, String, String, Int32, Int32, String, Int32, DataType, Int32, DataWidth, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_UpdateHdataChannelsDto__ctor_System_Int64_System_String_System_String_System_String_System_Int32_System_Int32_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public UpdateHdataChannelsDto(long uid, string channelName, string unit, string description, int integraldigits, int fractionalDigits, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, int mainAddress, int subAddress, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | uid | Uid |
| System.String | channelName | 通道名称 |
| System.String | unit | 单位 |
| System.String | description | 描述 |
| System.Int32 | integraldigits | 整数位 |
| System.Int32 | fractionalDigits | 小数位 |
| System.String | devAlias | PLC别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 |
| System.Int32 | regId | 寄存器Id |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 寄存器位宽 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 索引地址 |

### UpdateHdataChannelsDto\(Int64, String, String, String, Int32, String, Int32, DataType, String, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_UpdateHdataChannelsDto__ctor_System_Int64_System_String_System_String_System_String_System_Int32_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_String_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public UpdateHdataChannelsDto(long uid, string channelName, string unit, string description, int fractionalDigits, string devAlias, int stationNo, DataType dataType, string regName, int mainAddress, int subAddress, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | uid | Uid |
| System.String | channelName | 通道名称 |
| System.String | unit | 单位 |
| System.String | description | 描述 |
| System.Int32 | fractionalDigits | 小数位 |
| System.String | devAlias | PLC别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 索引地址 |

### UpdateHdataChannelsDto\(String, String, String, Int32, Int32, String, Int32, DataType, Int32, DataWidth, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_UpdateHdataChannelsDto__ctor_System_String_System_String_System_String_System_Int32_System_Int32_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_Int32_FBoxClientDriver_Contract_DataWidth_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public UpdateHdataChannelsDto(string channelName, string unit, string description, int integraldigits, int fractionalDigits, string devAlias, int stationNo, DataType dataType, int regId, DataWidth ioWidth, int mainAddress, int subAddress, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | channelName | 通道名称 |
| System.String | unit | 单位 |
| System.String | description | 描述 |
| System.Int32 | integraldigits | 整数位 |
| System.Int32 | fractionalDigits | 小数位 |
| System.String | devAlias | PLC别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 |
| System.Int32 | regId | 寄存器Id |
| [DataWidth](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataWidth.html) | ioWidth | 寄存器位宽 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 索引地址 |

### UpdateHdataChannelsDto\(String, String, String, Int32, String, Int32, DataType, String, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_UpdateHdataChannelsDto__ctor_System_String_System_String_System_String_System_Int32_System_String_System_Int32_FBoxClientDriver_Contract_DataType_System_String_System_Int32_System_Int32_System_Int32_"></a>

构造函数

#### Declaration

```text
public UpdateHdataChannelsDto(string channelName, string unit, string description, int fractionalDigits, string devAlias, int stationNo, DataType dataType, string regName, int mainAddress, int subAddress, int subIndex)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | channelName | 通道名称 |
| System.String | unit | 单位 |
| System.String | description | 描述 |
| System.Int32 | fractionalDigits | 小数位 |
| System.String | devAlias | PLC别名 |
| System.Int32 | stationNo | 站号 |
| [DataType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataType.html) | dataType | 数据类型 |
| System.String | regName | 寄存器名称 |
| System.Int32 | mainAddress | 主地址 |
| System.Int32 | subAddress | 子地址 |
| System.Int32 | subIndex | 索引地址 |

## Properties <a id="properties"></a>

### Uid <a id="FBoxClientDriver_Contract_UpdateHdataChannelsDto_Uid"></a>

Uid

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

