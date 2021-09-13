# Interface ICredentialProvider

密钥帮助接口

**Namespace: FBoxClientDriver.Contract**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_ICredentialProvider_syntax"></a>

```text
public interface ICredentialProvider
```

## Properties <a id="properties"></a>

### CacheDirectory <a id="FBoxClientDriver_Contract_ICredentialProvider_CacheDirectory"></a>

缓存路径

#### Declaration

```text
string CacheDirectory { get; set; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.String |  |

## Methods <a id="methods"></a>

### GetClientCredential\(\) <a id="FBoxClientDriver_Contract_ICredentialProvider_GetClientCredential"></a>

获取用户密钥信息

#### Declaration

```text
IClientCredential GetClientCredential()
```

#### Returns

| Type | Description |
| :--- | :--- |
| [IClientCredential](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.IClientCredential.html) |  |

### GetRefreshToken\(\) <a id="FBoxClientDriver_Contract_ICredentialProvider_GetRefreshToken"></a>

获取RefreshToken

#### Declaration

#### Returns

| Type | Description |
| :--- | :--- |
| System.String |  |

### GetUserCredential\(\) <a id="FBoxClientDriver_Contract_ICredentialProvider_GetUserCredential"></a>

获取用户信息

#### Declaration

```text
IUserCredential GetUserCredential()
```

#### Returns

| Type | Description |
| :--- | :--- |
| [IUserCredential](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.IUserCredential.html) |  |

### SetRefreshToken\(String\) <a id="FBoxClientDriver_Contract_ICredentialProvider_SetRefreshToken_System_String_"></a>

设置RefreshToken

#### Declaration

```text
void SetRefreshToken(string refreshtoken)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.String | refreshtoken |  |

