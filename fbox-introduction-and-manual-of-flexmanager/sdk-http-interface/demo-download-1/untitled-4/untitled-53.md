# ChangeBoxOwnerArgsV2

#### Inheritance

System.Object

ChangeBoxOwnerArgsV2

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

#### Syntax <a id="FBoxClientDriver_Contract_ChangeBoxOwnerArgsV2_syntax"></a>

```text
public class ChangeBoxOwnerArgsV2
```

## Constructors <a id="constructors"></a>

### ChangeBoxOwnerArgsV2\(String, String\) <a id="FBoxClientDriver_Contract_ChangeBoxOwnerArgsV2__ctor_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public ChangeBoxOwnerArgsV2(string boxNo, string targetUserName)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子号码 |
| System.String | targetUserName | 移交的对象用户名 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_ChangeBoxOwnerArgsV2_BoxNo"></a>

盒子号码

#### Declaration

```text
[JsonProperty("boxNo")]
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### TargetUserName <a id="FBoxClientDriver_Contract_ChangeBoxOwnerArgsV2_TargetUserName"></a>

移交的对象用户名

#### Declaration

```text
[JsonProperty("targetUserName")]
public string TargetUserName { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

