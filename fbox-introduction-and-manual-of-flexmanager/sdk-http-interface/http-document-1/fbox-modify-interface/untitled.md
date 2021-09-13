# Modify FBox Groups

* **Interface Function**

   This interface is used for users to add FBox groups

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL:**`[App Server]/api/client/boxgroup`

   **New Version：**

   **URL:**`[Host Server]/api/client/v2/box/group/mgt`

* **Address Request Parameter**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | App Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Request Mode**

  `POST`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Old Version Body**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | id | string | groupId \(obtained in the FBox list interface\) |
  | name | string | Group name  |

* **New Version Body**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | uid | string | groupId \(obtained in the FBox list interface\) |
  | name | string | Group name  |

* **Successful Response：**

   `NULL`

* **Return Code** 

  | Return Code | Description |
  | :--- | :--- |
  | 200 | successful request  |
  | 401 | accessToken expired  |
  | 404 | The interface does not exist or the FBox group does not exist |
  | 409 | Duplicate name  |

