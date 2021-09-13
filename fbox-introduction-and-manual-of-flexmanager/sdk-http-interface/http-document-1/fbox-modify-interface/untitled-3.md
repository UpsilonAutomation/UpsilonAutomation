# Modify the Refresh Interval of the Data-Saving Mode

* **Interface Function**

   This interface is used for users to globally modify the refresh interval of the data-saving mode.

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL：**`[apiBaseUrl]v2/box/{boxId}/boxSettings`

   **New Version：**

   **URL：** `[Host Server]/api/v2/box/{boxId}/boxSettings`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |

* **Request Mode**

   `POST`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**  
  The list collection, the properties of a single object are as follows.

   **body is a list of data monitoring points, transmitted in JSON format**  


  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | boxId | string | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | type | int | Fixed value, pass 0 |
  | value | int | Refresh interval \(unit/second\) |

* **Successful Response**

   null

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | execution succeed |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [appendix III ](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2)for details |
  | 429 | Access interface frequency is too fast |

