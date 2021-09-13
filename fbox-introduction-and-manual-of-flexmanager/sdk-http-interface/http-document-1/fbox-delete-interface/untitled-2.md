# Delete Monitoring Point Groups

* **Interface Function**

   This interface is used for user to delete monitoring point groups**.**

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL1：**`[apiBaseUrl]v2/box/{boxId}/dmon/group/{groupId}`

   **URL2：**`[apiBaseUrl]v2/box/dmon/group/{groupId}/?boxNo={boxNo}`

   **New Version:**

   **URL1：**`[Host Server]/api/v2/box/{boxId}/dmon/group/{groupId}`

   **URL2：**`[Host Server]v2/box/dmon/group/{groupId}/?boxNo={boxNo}`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | boxNo | long | Box serial number |
  | groupId | Long | Monitoring group Id |

* **Request Mode**

   `DELETE`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

   `NULL`

* **Successful Response**

   `NULL`

* **Response failed**

  | Return Code | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 304 | Monitoring point group does not exist |
  | 424 | FBox is not online |
  | 500 | Interface internal error |

