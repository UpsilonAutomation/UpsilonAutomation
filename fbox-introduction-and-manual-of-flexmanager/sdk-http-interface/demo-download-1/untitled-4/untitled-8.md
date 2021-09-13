# AddHdataItemDto

新增历史记录多通道参数

#### Inheritance

System.Object

AddHdataItemDto

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

#### Syntax <a id="FBoxClientDriver_Contract_AddHdataItemDto_syntax"></a>

```text
public class AddHdataItemDto : HdataItemDto
```

## Constructors <a id="constructors"></a>

### AddHdataItemDto\(\) <a id="FBoxClientDriver_Contract_AddHdataItemDto__ctor"></a>

ctor

#### Declaration

### AddHdataItemDto\(String, Int32, Boolean, HDataControlOptionsV2, IList\) <a id="FBoxClientDriver_Contract_AddHdataItemDto__ctor_System_String_System_Int32_System_Boolean_FBoxClientDriver_Contract_HDataControlOptionsV2_System_Collections_Generic_IList_FBoxClientDriver_Contract_AddHdataChannelsDto__"></a>

ctor

#### Declaration

```text
public AddHdataItemDto(string name, int recordingPeriod, bool isControl, HDataControlOptionsV2 controlOptions, IList hdataChannels)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | name |  |
| System.Int32 | recordingPeriod |  |
| System.Boolean | isControl |  |
| [HDataControlOptionsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HDataControlOptionsV2.html) | controlOptions |  |
| System.Collections.Generic.IList&lt;[AddHdataChannelsDto](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHdataChannelsDto.html)&gt; | hdataChannels |  |

## Properties <a id="properties"></a>

### HdataChannels <a id="FBoxClientDriver_Contract_AddHdataItemDto_HdataChannels"></a>

通道集合

#### Declaration

```text
[JsonProperty("channels")]
public IList HdataChannels { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[AddHdataChannelsDto](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHdataChannelsDto.html)&gt; |  |

