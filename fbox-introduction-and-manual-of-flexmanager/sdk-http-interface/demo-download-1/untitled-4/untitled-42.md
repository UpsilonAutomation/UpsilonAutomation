# BoxDMonGroupsDtoV2

监控点分组

#### Inheritance

System.Object

BoxDMonGroupsDtoV2

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

#### Syntax <a id="FBoxClientDriver_Contract_BoxDMonGroupsDtoV2_syntax"></a>

```text
public class BoxDMonGroupsDtoV2
```

## Constructors <a id="constructors"></a>

### BoxDMonGroupsDtoV2\(\) <a id="FBoxClientDriver_Contract_BoxDMonGroupsDtoV2__ctor"></a>

构造函数

#### Declaration

```text
public BoxDMonGroupsDtoV2()
```

## Properties <a id="properties"></a>

### Id <a id="FBoxClientDriver_Contract_BoxDMonGroupsDtoV2_Id"></a>

监控点分组Id

#### Declaration

```text
public long Id { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### Items <a id="FBoxClientDriver_Contract_BoxDMonGroupsDtoV2_Items"></a>

监控点条目集合

#### Declaration

```text
public IList Items { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[DmonItemDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DmonItemDtoV2.html)&gt; |  |

### Name <a id="FBoxClientDriver_Contract_BoxDMonGroupsDtoV2_Name"></a>

监控点名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

