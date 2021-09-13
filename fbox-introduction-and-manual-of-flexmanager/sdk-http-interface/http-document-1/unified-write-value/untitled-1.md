# Unified Write Group Write Value

* **Function Description**

  Unified write values for the monitoring points under the unified write group, and the value value is the type specified in the unified write group

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL:**`[apiBaseUrl]/v2/control/group/write/value`

   **New Version：**

   **URL:**`[Host Server]/api/v2/control/group/write/value`

* **Address Parameter Description**

  | Parameter Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Method**

   `POST`

* **Headers：**

  | Filed Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

  | Parameter Name | Type | Description |
  | :--- | :--- | :--- |
  |  value | int | Value, the type specified in the unified write group |
  |  uid | string | Write group Id uniformly, choose one of group name |
  |  name | string | Write the group name uniformly, choose one of the group IDs, and give priority to the group name |

* **Return Field**

   `Null`

* **Return Code**

  | Return Code | Description |
  | :--- | :--- |
  | 401 | refresh\_token expired or wrong |
  | 429 | Rejected by the server \(login is too frequent, the client is banned, etc.\) |

