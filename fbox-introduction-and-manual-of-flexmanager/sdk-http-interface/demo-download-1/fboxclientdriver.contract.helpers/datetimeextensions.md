# DateTimeExtensions

时间扩展方法

#### Inheritance

System.Object

DateTimeExtensions

#### Inherited Members

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver.Contract.Helpers**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_Helpers_DateTimeExtensions_syntax"></a>

```text
public static class DateTimeExtensions
```

## Methods <a id="methods"></a>

### FromJsEpoch\(Int64\) <a id="FBoxClientDriver_Contract_Helpers_DateTimeExtensions_FromJsEpoch_System_Int64_"></a>

#### Declaration

```text
public static DateTime FromJsEpoch(long jsTime)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | jsTime |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.DateTime |  |

### JsEpochTime\(DateTime\) <a id="FBoxClientDriver_Contract_Helpers_DateTimeExtensions_JsEpochTime_System_DateTime_"></a>

#### Declaration

```text
public static long JsEpochTime(this DateTime dateTime)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.DateTime | dateTime |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### UnixEpochTime\(DateTime\) <a id="FBoxClientDriver_Contract_Helpers_DateTimeExtensions_UnixEpochTime_System_DateTime_"></a>

#### Declaration

```text
public static long UnixEpochTime(this DateTime dateTime)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.DateTime | dateTime |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

