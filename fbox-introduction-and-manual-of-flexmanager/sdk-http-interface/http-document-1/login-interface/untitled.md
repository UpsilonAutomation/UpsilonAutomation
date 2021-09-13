# User Login

## Method 1`(The developer account created on the Managerplatform can only be used for one pass)` <a id="&#x65B9;&#x5F0F;&#x4E00;&#x5728;manager&#x5E73;&#x53F0;&#x4E0A;&#x521B;&#x5EFA;&#x7684;&#x5F00;&#x53D1;&#x8005;&#x8D26;&#x53F7;&#x53EA;&#x80FD;&#x7528;&#x65B9;&#x5F0F;&#x4E00;&#x4F20;&#x53C2;"></a>

* **Interface Function**

  This interface is used to obtain accessToken.

   **NOTE：**  
   The validity period of the obtained accessToken is 2 hours, and the validity period of refreshToken is 30 days. If a 401 error occurs in the calling interface, call the re-login interface to refresh the accessToken through refreshToken. A certain frequency will block IP processing.  
  **NOTE:**  
  All interfaces in this document do not support cross-domain requests

* **Request Address:（pick one of two）**

  **New version：**

  **URL:**`[Host Server]/idserver/core/connect/token`

  **Old version：**

  **URL:**`[Id Server]/core/connect/token`

* **Address Parameter Description**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | Id Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Method**

  `POST`

* **Headers**

  `NULL`

* **Body**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | scope | string | fbox |
  | client\_id | string | developer ID |
  | client\_secret | string | Original key |
  | grant\_type | string | client\_credentials |

 **NOTE：**

 The Content-Type \(body format\) of the login interface and the re-login interface is application/x-www-form-urlencoded The format of other interface body is application/json format.

 `client_id`, `client_secret`the developer ID and key created on the Manager platform. For details, see **Developer Creation**.

 `scope`and `grant_type`are the fixed value stated in the description.

* **Return Field**

  | Field Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | access\_Token | string | accessToken |
  | expires\_in | int | Validity period of accessToken |
  | refresh\_Token | string | After accessToken turn invalid，refresh accessToken |
  | token\_type | string | Type of accessToken \(Bearer\) fixed value |

* **Return Code**

  | Return Code | Description |
  | :--- | :--- |
  | 400 | "error\_description"="invalid\_username\_or\_password" \(account or password error\) Or "error": "invalid\_client" \(the developer account or password is wrong\) |
  | 404 | The interface does not exist, please check the URL |
  | 429 | Rejected by the server \(login is too frequent, the client is banned, etc.\) |

* \*\*\*\*[**The call case is as shown below**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/clientscertr5.png)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2860%29.png)

## Method 2:`(The developer account applied for sales to our company can only be transferred in the seconds method)` <a id="&#x65B9;&#x5F0F;&#x4E8C;&#x5411;&#x6211;&#x53F8;&#x9500;&#x552E;&#x7533;&#x8BF7;&#x7684;&#x5F00;&#x53D1;&#x8005;&#x8D26;&#x53F7;&#x53EA;&#x80FD;&#x7528;&#x65B9;&#x5F0F;&#x4E8C;&#x65B9;&#x5F0F;&#x4F20;&#x53C2;"></a>

* **Interface Function**

  The interface is used to obtain accessToken.

   **NOTE：**  
  The validity period of the obtained accessToken is 2 hours, and the validity period of refreshToken is 30 days. If a 401 error occurs in the calling interface, call the re-login interface to refresh the accessToken through refreshToken. A certain frequency will block IP processing.  
  **NOTE:**  
  All interfaces in this document do not support cross-domain requests

* **Request address：（pick one of two）**

  **New version：**

  **URL:**`[Host Server]/idserver/core/connect/token`

  **Old version：**

  **URL:**`[Id Server]/core/connect/token`

* **Parameter Description**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | Id Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Method**

  `POST`

* **Headers**

  `NULL`

* **Body**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | username | string | FBox client account |
  | password | string | FBox client password |
  | scope | string | openid offline\_access fbox email profile |
  | client\_id | string | developer account |
  | client\_secret | string | developer password |
  | grant\_type | string | password |

  **NOTE ：**  
  The Content-Type \(body format\) of the login interface and the re-login interface is application/x-www-form-urlencoded The format of other interface body is application/json format.

  `username`,`password`are the username and password of FlexManager, please download and login [FlexManager](http://fs.flexem.com/Box/en) by yourself. 

  `client_id`,`client_secret`are the developer account and password created by the server for various clients are used to distinguish various clients. Please contact the sales company that connects to your company to obtain them.

  `scope`and`grant_type`are the fixed value described in the description.

* **Return Field**

  | Field Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | access\_Token | string | accessToken |
  | expires\_in | int | Validity period of accessToken |
  | refresh\_Token | string | After the accessToken expires, refresh the accessToken |
  | token\_type | string | Type of accessToken \(Bearer\) fixed value |

* **Return Code**

  | Return Code | Description |
  | :--- | :--- |
  | 400 | "error\_description"="invalid\_username\_or\_password" \(account or password error\) Or "error": "invalid\_client" \(the developer account or password is wrong\) |
  | 404 | The interface does not exist, please check the URL |
  | 429 | Rejected by the server \(login is too frequent, the client is banned, etc.\) |

* \*\*\*\*[**The call case is as shown below**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/Login.png)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2862%29.png)

