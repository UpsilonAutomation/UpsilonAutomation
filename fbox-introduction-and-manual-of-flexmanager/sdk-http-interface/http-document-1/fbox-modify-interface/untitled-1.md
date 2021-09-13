# Modify FBox Name

* **Interface Function**

  This interface is used for users to add FBox names.

* **Request Address \(pick one of two\)**

  **Old Version：**

  **URL:**`[App Server]/api/client/v2/box/{boxId}/alias`

  **New Versios：**

  **URL:**`[Host Server]/api/client/v2/box/{boxId}/alias`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | App Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | long | Box id |

* **Request Mode**

  `POST`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | alias | string | Modify FBox name |

* **Successful Response**

  **：**

  `NULL`

* **Return Code**

  | Return Code | Description |
  | :--- | :--- |
  | 200 | Request succeeded |
  | 401 | accessToken expired |
  | 404 | The interface does not exist or the FBox group does not exist |
  | 409 | Duplicate name  |

