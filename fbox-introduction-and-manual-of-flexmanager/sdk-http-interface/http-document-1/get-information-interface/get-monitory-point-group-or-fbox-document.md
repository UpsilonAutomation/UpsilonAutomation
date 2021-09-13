# Get Monitory Point Group

* **Function Description**

   This interface can be used for users to obtain monitoring point groups.。

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL1:** `[apiBaseUrl]v2/box/{boxId}/dmon/groups`

   **URL2:** `[apiBaseUrl]v2/box/dmon/groups?boxNo={boxNo}`

   **New Version**

   **URL1:**`[Host Server]/api/v2/box/{boxId}/dmon/groups`

   **URL2:**`[Host Server]/api/v2/box/dmon/groups?boxNo={boxNo}`

* **Address Paramter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | Uid | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | boxNo | string | FBox serial numer |

* **Request Mode**

   `GET`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

   `NULL`

* **Return Filed**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | id | string | Monitoring point group Id |
  | name | string | Monitoring point group name |

* Return Code

  | Field Name | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 404 | The interface does not exist, please check the URL |
  | 429 | Access interface too frequently |

  |  |
  | :--- |

