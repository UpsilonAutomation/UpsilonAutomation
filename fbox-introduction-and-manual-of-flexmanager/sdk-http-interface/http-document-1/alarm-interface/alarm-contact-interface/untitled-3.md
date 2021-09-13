# Modify Alarm Contact

* **Function Description**

   The interface is used for users to modify alarm contact

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL:**`[apiBaseUrl]v2/contact`

   **New Version：**

   **URL:**`[Host Server]/api/v2/contact`

* **Address Parameter Description**

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
  | uid | string | Alarm contact uid |
  | email | string | Alarm contact email |
  | name | string | Alarm contact name |
  | cellphone | string | Alarm contact mobile number |
  | enabled | boolean | whether to enable  |
  | noticeType | int | 0：non 1：SMS，2：voice，3：voice and SMS |
  | memo | string | Remark |

* **Successful Response**

   `NULL`

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 409 | Name conflicts |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |

