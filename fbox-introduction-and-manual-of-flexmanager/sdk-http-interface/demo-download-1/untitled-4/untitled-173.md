# UpdateTargetArgs

更新报警联系人参数

#### Inheritance

System.Object

UpdateTargetArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UpdateTargetArgs_syntax"></a>

```text
public class UpdateTargetArgs
```

## Constructors <a id="constructors"></a>

### UpdateTargetArgs\(\) <a id="FBoxClientDriver_Contract_UpdateTargetArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public UpdateTargetArgs()
```

### UpdateTargetArgs\(Int64, String, String, String, String, Boolean, IList\) <a id="FBoxClientDriver_Contract_UpdateTargetArgs__ctor_System_Int64_System_String_System_String_System_String_System_String_System_Boolean_System_Collections_Generic_IList_System_Int64__"></a>

构造函数

#### Declaration

```text
public UpdateTargetArgs(long uid, string boxNo, string name, string cellphone, string email, bool enabled, IList alarmGroupUidList)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | uid | 报警联系人UID |
| System.String | boxNo | 盒子编码 |
| System.String | name | 报警联系人名称 |
| System.String | cellphone | 电话号码 |
| System.String | email | 电子邮件 |
| System.Boolean | enabled | 是否可用 |
| System.Collections.Generic.IList&lt;System.Int64&gt; | alarmGroupUidList | 所属报警组别列表 |

## Properties <a id="properties"></a>

### AlarmGroupUidList <a id="FBoxClientDriver_Contract_UpdateTargetArgs_AlarmGroupUidList"></a>

所属报警组别列表

#### Declaration

```text
public IList AlarmGroupUidList { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; |  |

### BoxNo <a id="FBoxClientDriver_Contract_UpdateTargetArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Cellphone <a id="FBoxClientDriver_Contract_UpdateTargetArgs_Cellphone"></a>

电话号码

#### Declaration

```text
public string Cellphone { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Email <a id="FBoxClientDriver_Contract_UpdateTargetArgs_Email"></a>

电子邮件

#### Declaration

```text
public string Email { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Enabled <a id="FBoxClientDriver_Contract_UpdateTargetArgs_Enabled"></a>

是否可用

#### Declaration

```text
public bool Enabled { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Memo <a id="FBoxClientDriver_Contract_UpdateTargetArgs_Memo"></a>

备注

#### Declaration

```text
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_UpdateTargetArgs_Name"></a>

报警联系人名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Uid <a id="FBoxClientDriver_Contract_UpdateTargetArgs_Uid"></a>

报警联系人UID

#### Declaration

```text
public long Uid { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

