# Query All Unified Writing Groups

* **Function Description**

   可以获取账号下的所有统一写分组

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL:**`[apiBaseUrl]/v2/control/groups`

   **New Version：**

   **URL:**`[Host Server]/api/v2/control/groups`

* **Address Parameter Description**

  | Parameter Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Method**

   `GET`

* **Headers：**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   `Null`

* **Return Filed**

  | Parameter Name | Type | Description |
  | :--- | :--- | :--- |
  |  name | string | 组名称 |
  |  type | string | 组数据类型 |
  |  uid | string | 统一写组Id |

* **Return Code**

  | Return Code | Description |
  | :--- | :--- |
  | 401 | refresh\_token过期或者错误 |
  | 404 | 接口不存在，请检查URL |
  | 429 | 被服务器拒绝（登录过于频繁，客户端被禁止等） |

