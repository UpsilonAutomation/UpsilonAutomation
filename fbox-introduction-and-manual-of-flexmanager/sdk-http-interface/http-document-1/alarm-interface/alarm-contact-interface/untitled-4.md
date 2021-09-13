# Delete Alarm Contact

* **Function Description**

   The interface is used for users to delete alarm contact

* **Request Address \(pick of two\)** 

   **Old Version：**

   **URL:**`[apiBaseUrl]v2/contact/{uid}`

   **New Version：**

   **URL:**`[Host Server]/api/v2/contact/{uid}`

* **Address Parameter Descriprtion**

  |  | Field Name | Type |  | Description |
  | :--- | :--- | :--- | :--- | :--- |
  |  | apiBaseUrl | string |  | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  |  | uid | Long |  | uid main key of alarm contact |

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

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 404 | Alarm contact does not exist |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |

