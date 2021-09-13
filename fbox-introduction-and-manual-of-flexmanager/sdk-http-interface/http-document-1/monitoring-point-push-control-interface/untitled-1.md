# Pause A Monitoring Point Group

* **Function Description**

   After calling this interface, the current signalr real-time data push event will not receive the monitoring point data under a certain monitoring point group under the box

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL:**`[apiBaseUrl]dmon/group/{gid}/stop`

   **New Version：**

   **URL:**`[Host Server]/api/dmon/group/{gid}/stop`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | gid | string | 监控点组别uid |

* **Request Mode**

   `POST`

* **Header**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

   `NULL`

* Successful Response

   `NULL`

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 429 | Access interface frequency is too fast |

