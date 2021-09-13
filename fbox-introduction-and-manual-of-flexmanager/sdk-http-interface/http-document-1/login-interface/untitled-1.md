# Re-Login in the Old Version

* **Interface Function**

   The Token has expired, if you have successfully logged in and the refresh\_token is valid, the interface is preferred to refresh the Token

* **Request address：（pick one of two）**

   **Old Version：**

   **URL:**`[Id Server]/core/connect/token`

   **New Version：**

   **URL:**`[Host Server]/idserver/core/connect/token`

* **Address parameter Description**

  | Parameter Name | Parameter Type | Parameter Description |
  | :--- | :--- | :--- |
  | Id Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Method**

  `POST`

* **Headers：**

   `NULL`

* **Body**

  | Parameter Name | Parameter Type | Parameter Description |
  | :--- | :--- | :--- |
  |  refresh\_token | string | Refresh\_token obtained from the login interface |
  |  scope | string | openid offline\_access fbox email profile |
  |  client\_id | string | Client ID |
  |  client\_secret | string | Client password |
  |  grant\_type | string | refresh\_token |

   **NOTE ：**  
   The Content-Type of HTTP \(body format\) is application/x-www-form-urlencoded

   client\_id\client\_secret is the user name and password created by the server for various clients, which are used to distinguish various clients. Please contact the sales partner of your company to obtain them.

   `scopea and grant_type`are the fixed value stated in the description.

* **Return Filed** 

  | Filed Name | Type | Description |
  | :--- | :--- | :--- |
  | access\_token | string | accessToken |
  | expires\_in | int | valid period of accessToken |
  | refresh\_token | string | After the accessToken expires, refresh the accessToken |
  | token\_type | string | Type of accessToken \(Bearer\) fixed value |

* **Return Code**

  | Return Code | Description |
  | :--- | :--- |
  | 401 | refresh\_token expired or wrong |
  | 429 | Rejected by the server \(login is too frequent, the client is banned, etc.\) |

  **NOTE:**  
   Login interface returns `invalid_type`OR`invalid_grant`are both the login information is wrong.

\*\*\*\*[**The call case is as follows:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/clientscertr4.png)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2846%29.png)

