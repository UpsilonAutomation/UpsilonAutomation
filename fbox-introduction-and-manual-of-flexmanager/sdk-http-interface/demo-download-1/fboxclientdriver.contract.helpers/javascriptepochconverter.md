# JavascriptEpochConverter

#### Inheritance

System.Object

Newtonsoft.Json.JsonConverter

Newtonsoft.Json.Converters.DateTimeConverterBase

JavascriptEpochConverter

#### Inherited Members

Newtonsoft.Json.Converters.DateTimeConverterBase.CanConvert\(System.Type\)

Newtonsoft.Json.JsonConverter.CanRead

Newtonsoft.Json.JsonConverter.CanWrite

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver.Contract.Helpers**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_Helpers_JavascriptEpochConverter_syntax"></a>

```text
public class JavascriptEpochConverter : DateTimeConverterBase
```

## Methods <a id="methods"></a>

### ReadJson\(JsonReader, Type, Object, JsonSerializer\) <a id="FBoxClientDriver_Contract_Helpers_JavascriptEpochConverter_ReadJson_Newtonsoft_Json_JsonReader_System_Type_System_Object_Newtonsoft_Json_JsonSerializer_"></a>

#### Declaration

```text
public override object ReadJson(JsonReader reader, Type objectType, object existingValue, JsonSerializer serializer)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| Newtonsoft.Json.JsonReader | reader |  |
| System.Type | objectType |  |
| System.Object | existingValue |  |
| Newtonsoft.Json.JsonSerializer | serializer |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Object |  |

#### Overrides

Newtonsoft.Json.JsonConverter.ReadJson\(Newtonsoft.Json.JsonReader, System.Type, System.Object, Newtonsoft.Json.JsonSerializer\)

### WriteJson\(JsonWriter, Object, JsonSerializer\) <a id="FBoxClientDriver_Contract_Helpers_JavascriptEpochConverter_WriteJson_Newtonsoft_Json_JsonWriter_System_Object_Newtonsoft_Json_JsonSerializer_"></a>

#### Declaration

```text
public override void WriteJson(JsonWriter writer, object value, JsonSerializer serializer)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| Newtonsoft.Json.JsonWriter | writer |  |
| System.Object | value |  |
| Newtonsoft.Json.JsonSerializer | serializer |  |

#### Overrides

Newtonsoft.Json.JsonConverter.WriteJson\(Newtonsoft.Json.JsonWriter, System.Object, Newtonsoft.Json.JsonSerializer\)

