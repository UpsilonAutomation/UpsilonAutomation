# Delete FBox Groups

* **Interface Function**

   The interface is used for users to delete FBox groups.

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL:**`[App Server]/api/client/group/{groupId}`

   **New Version：**

   **URL:**`[Host Server]/api/client/group/{groupId}`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | App Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | groupId | Long | Group id The id of the largest grouping unit in the FBox list is the groupId |

* **Request Mode**

  `DELETE`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

   `NULL`

* **Successful Response：**

   `NULL`

* **Return Code**

  | Return Code | Description |
  | :--- | :--- |
  | 200 | request succeeded |
  | 401 | accessToken expired |
  | 404 | The interface does not exist or the FBox group does not exist |
  | 406 | Cannot delete the last group |

