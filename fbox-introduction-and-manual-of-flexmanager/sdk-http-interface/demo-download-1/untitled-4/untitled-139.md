# UnregisterBoxArgs

删除注册盒子信息参数

#### Inheritance

System.Object

UnregisterBoxArgs

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

#### Syntax <a id="FBoxClientDriver_Contract_UnregisterBoxArgs_syntax"></a>

```text
public class UnregisterBoxArgs
```

## Constructors <a id="constructors"></a>

### UnregisterBoxArgs\(\) <a id="FBoxClientDriver_Contract_UnregisterBoxArgs__ctor"></a>

无参构造函数

#### Declaration

```text
public UnregisterBoxArgs()
```

### UnregisterBoxArgs\(String, String\) <a id="FBoxClientDriver_Contract_UnregisterBoxArgs__ctor_System_String_System_String_"></a>

构造函数

#### Declaration

```text
public UnregisterBoxArgs(string boxNo, string boxPassword = null)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | boxNo | 盒子编码 |
| System.String | boxPassword | 盒子密码 |

## Properties <a id="properties"></a>

### BoxNo <a id="FBoxClientDriver_Contract_UnregisterBoxArgs_BoxNo"></a>

盒子编码

#### Declaration

```text
public string BoxNo { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

### BoxPassword <a id="FBoxClientDriver_Contract_UnregisterBoxArgs_BoxPassword"></a>

盒子密码

#### Declaration

```text
public string BoxPassword { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

