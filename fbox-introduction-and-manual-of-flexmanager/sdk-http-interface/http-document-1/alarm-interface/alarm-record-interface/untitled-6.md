# Confirm Alarm

* **Request Address** 

   **Old Version \(pick one of two\)**

   **URL:**`[apiBaseUrl]alarm/{uid}/confirm`

   **New Version：**

   **URL:**`[Host Server]/api/alarm/{uid}/confirm`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | Uid | Long | Main key uid of alarm entry  |

* **Request Mode**

   `POST`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   `NULL`

* **Successful Response**

   `NULL`

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | Execution succeed |
  | 401 | accessToken expired  |
  | 404 | Interface does not exist, please check URL |
  | 429 | Access interface frequency is too fast |

