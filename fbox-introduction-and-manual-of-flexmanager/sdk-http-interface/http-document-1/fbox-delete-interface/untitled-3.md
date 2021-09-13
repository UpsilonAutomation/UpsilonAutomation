# Delete Data Monitoring Points

* **Interface Function**

   The interface is used for users to delete data monitoring points.

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL1：**`[apiBaseUrl]v2/box/{boxId}/dmon/del`

   **URL2：**`[apiBaseUrl]v2/box/dmon/del?boxNo={boxNo}`

   **New Version:**

   **URL1：**`[Host Server]/api/v2/box/{boxId}/dmon/del`

   **URL2：**`[Host Server]/api/v2/box/{boxId}/dmon/del`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | boxNo | string | FBox serial number |

* **Request Mode**

   `POST`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   Monitoring point Uid collection（JSON transmission）

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | Execution succeed  |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
  | 429 | Access interface frequency is too fast |

