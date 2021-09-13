# Delete Alarm Groups

* **Function Description**

   The interface is used for users to delete alarm groups.

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL:**`[apiBaseUrl]v2/alarm/group/del`

   **New Versions：**

   **URL:**`[Host Server]/api/v2/alarm/group/del`

* **Address Parameter Description:**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

  * **Request Mode**

     `POST`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | uid | long | 为报警分组的uid主键 |
  | boxId | long | 盒子id |

* **Successful Response**

   `NULL`

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 404 | Alarm group does not exist |
  | 416 | The last group cannot be deleted |
  | 406 | There are alarm entries that cannot be deleted |

