# Delete Historical Record

* **Function Description**

   The interface is used for users to delete historical record

* **Request Address \(pick one of two\)**

   **Old version:**

   **URL1:** `[apiBaseUrl]v2/box/{boxId}/hdataitems/del`

   **URL2:** `[apiBaseUrl]v2/hdataitems/del?boxNo={boxNo}`

   **New Version:**

   **URL1:**`[Host Server]/api/v2/box/{boxId}/hdataitems/del`

   **URL2:**`[Host Server]/api/v2/hdataitems/del?boxNo={boxNo}`

* **Parameter Description:**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxid | Long | uid main key of alarm contact |
  | boxNo | string | FBox serial number |

* **Request Mode**

   `POST`

* **Header**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface  |

* **Body**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | ids | long collection | History record id collection, choose one from names |
  | names | string collection | History record name collection, choose one from Ids |

* **Successful Response**

   `NULL`

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | Execution succeed |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
  | 429 | Access interface frequency is too fast |

