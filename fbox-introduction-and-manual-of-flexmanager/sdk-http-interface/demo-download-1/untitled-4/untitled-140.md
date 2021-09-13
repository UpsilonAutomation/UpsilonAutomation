# RegisterBoxArgs

注册盒子参数

#### Inheritance

System.Object

RegisterBoxArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_RegisterBoxArgs_syntax"></a>

```text
public class RegisterBoxArgs
```

## Constructors <a id="constructors"></a>

### RegisterBoxArgs\(\) <a id="FBoxClientDriver_Contract_RegisterBoxArgs__ctor"></a>

无参构造函数

#### Declaration

### RegisterBoxArgs\(Int64, String, String, String\) <a id="FBoxClientDriver_Contract_RegisterBoxArgs__ctor_System_Int64_System_String_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public RegisterBoxArgs(long boxGroupId, string boxPassword, string boxNo, string alias)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int64 | boxGroupId | 盒子组别ID |
| System.String | boxPassword | 盒子密码 |
| System.String | boxNo | 盒子编码 |
| System.String | alias |  |

### RegisterBoxArgs\(String, String, String, String\) <a id="FBoxClientDriver_Contract_RegisterBoxArgs__ctor_System_String_System_String_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public RegisterBoxArgs(string boxNo, string boxPassword, string alias, string groupName)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.String | boxPassword | 盒子密码 |
| System.String | alias | 别名 |
| System.String | groupName | 监控点分组名称 |

## Properties <a id="properties"></a>

### Alias <a id="FBoxClientDriver_Contract_RegisterBoxArgs_Alias"></a>

盒子名称

#### Declaration

```text
public string Alias { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxGroupId <a id="FBoxClientDriver_Contract_RegisterBoxArgs_BoxGroupId"></a>

盒子分组Id

#### Declaration

```text
public long BoxGroupId { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Int64 |  |

### BoxNo <a id="FBoxClientDriver_Contract_RegisterBoxArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxPassword <a id="FBoxClientDriver_Contract_RegisterBoxArgs_BoxPassword"></a>

盒子密码

#### Declaration

```text
public string BoxPassword { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### GroupName <a id="FBoxClientDriver_Contract_RegisterBoxArgs_GroupName"></a>

盒子分组名称

#### Declaration

```text
public string GroupName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

