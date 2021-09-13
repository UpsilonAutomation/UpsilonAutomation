# UpdateRefreshTimeArgs

更新刷新时间参数

#### Inheritance

System.Object

UpdateRefreshTimeArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateRefreshTimeArgs_syntax"></a>

```text
public class UpdateRefreshTimeArgs
```

## Constructors <a id="constructors"></a>

### UpdateRefreshTimeArgs\(\) <a id="FBoxClientDriver_Contract_UpdateRefreshTimeArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public UpdateRefreshTimeArgs()
```

### UpdateRefreshTimeArgs\(String, Int32\) <a id="FBoxClientDriver_Contract_UpdateRefreshTimeArgs__ctor_System_String_System_Int32_"></a>

构造函数

#### Declaration

```text
public UpdateRefreshTimeArgs(string boxNo, int intervalTime)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.Int32 | intervalTime | 刷新时间 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_UpdateRefreshTimeArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### IntervalTime <a id="FBoxClientDriver_Contract_UpdateRefreshTimeArgs_IntervalTime"></a>

刷新时间

#### Declaration

```text
public int IntervalTime { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int32 |  |

