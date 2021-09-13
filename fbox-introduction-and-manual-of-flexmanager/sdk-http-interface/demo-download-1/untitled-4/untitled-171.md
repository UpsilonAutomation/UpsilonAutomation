# UpdateHdataItemDto

历史记录更新对象

#### Inheritance

System.Object

UpdateHdataItemDto

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateHdataItemDto_syntax"></a>

```text
public class UpdateHdataItemDto : HdataItemDto
```

## Constructors <a id="constructors"></a>

### UpdateHdataItemDto\(\) <a id="FBoxClientDriver_Contract_UpdateHdataItemDto__ctor"></a>

构造函数

#### Declaration

```text
public UpdateHdataItemDto()
```

### UpdateHdataItemDto\(Int64, String, Int32, Boolean, HDataControlOptionsV2, IList\) <a id="FBoxClientDriver_Contract_UpdateHdataItemDto__ctor_System_Int64_System_String_System_Int32_System_Boolean_FBoxClientDriver_Contract_HDataControlOptionsV2_System_Collections_Generic_IList_FBoxClientDriver_Contract_UpdateHdataChannelsDto__"></a>

构造函数

#### Declaration

```text
public UpdateHdataItemDto(long uid, string name, int recordingPeriod, bool isControl, HDataControlOptionsV2 controlOptions, IList hdataChannels)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | uid | Uid |
| System.String | name | 名称 |
| System.Int32 | recordingPeriod | 采集周期 |
| System.Boolean | isControl | 是否启用使能 |
| [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) | controlOptions | 使能参数 |
| System.Collections.Generic.IList&lt;[UpdateHdataChannelsDto](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataChannelsDto.html)&gt; | hdataChannels | 多通道 |

### UpdateHdataItemDto\(String, Int32, Boolean, HDataControlOptionsV2, IList\) <a id="FBoxClientDriver_Contract_UpdateHdataItemDto__ctor_System_String_System_Int32_System_Boolean_FBoxClientDriver_Contract_HDataControlOptionsV2_System_Collections_Generic_IList_FBoxClientDriver_Contract_UpdateHdataChannelsDto__"></a>

#### Declaration

```text
public UpdateHdataItemDto(string name, int recordingPeriod, bool isControl, HDataControlOptionsV2 controlOptions, IList hdataChannels)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name |  |
| System.Int32 | recordingPeriod |  |
| System.Boolean | isControl |  |
| [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) | controlOptions |  |
| System.Collections.Generic.IList&lt;[UpdateHdataChannelsDto](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataChannelsDto.html)&gt; | hdataChannels |  |

## Properties <a id="properties"></a>

### HdataChannels <a id="FBoxClientDriver_Contract_UpdateHdataItemDto_HdataChannels"></a>

通道集合

#### Declaration

```text
[JsonProperty("channels")]
public IList HdataChannels { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[UpdateHdataChannelsDto](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataChannelsDto.html)&gt; |  |

### Uid <a id="FBoxClientDriver_Contract_UpdateHdataItemDto_Uid"></a>

Uid

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

