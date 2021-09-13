# AddTargetArgs

新增报警联系人参数

#### Inheritance

System.Object

AddTargetArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_AddTargetArgs_syntax"></a>

```text
public class AddTargetArgs
```

## Constructors <a id="constructors"></a>

### AddTargetArgs\(\) <a id="FBoxClientDriver_Contract_AddTargetArgs__ctor"></a>

无参构造函数

#### Declaration

### AddTargetArgs\(String, String, String, String, Boolean, IList\) <a id="FBoxClientDriver_Contract_AddTargetArgs__ctor_System_String_System_String_System_String_System_String_System_Boolean_System_Collections_Generic_IList_System_Int64__"></a>

构造函数

#### Declaration

```text
public AddTargetArgs(string boxNo, string name, string cellphone, string email, bool enable, IList alarmGroupUidList)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.String | name | 报警联系人名称 |
| System.String | cellphone | 报警联系人电话 |
| System.String | email | 报警联系人邮箱 |
| System.Boolean | enable | 是否启用 |
| System.Collections.Generic.IList&lt;System.Int64&gt; | alarmGroupUidList | 报警联系所属的组别 |

## Properties <a id="properties"></a>

### AlarmGroupUidList <a id="FBoxClientDriver_Contract_AddTargetArgs_AlarmGroupUidList"></a>

报警联系所属的组别

#### Declaration

```text
public IList AlarmGroupUidList { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;System.Int64&gt; |  |

### BoxNo <a id="FBoxClientDriver_Contract_AddTargetArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Cellphone <a id="FBoxClientDriver_Contract_AddTargetArgs_Cellphone"></a>

报警联系人电话

#### Declaration

```text
public string Cellphone { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Email <a id="FBoxClientDriver_Contract_AddTargetArgs_Email"></a>

报警联系人邮箱

#### Declaration

```text
public string Email { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Enable <a id="FBoxClientDriver_Contract_AddTargetArgs_Enable"></a>

是否启用

#### Declaration

```text
public bool Enable { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Boolean |  |

### Memo <a id="FBoxClientDriver_Contract_AddTargetArgs_Memo"></a>

备注

#### Declaration

```text
public string Memo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### Name <a id="FBoxClientDriver_Contract_AddTargetArgs_Name"></a>

报警联系人名称

#### Declaration

```text
public string Name { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

