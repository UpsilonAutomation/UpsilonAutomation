# Only Open A Monitoring Point Group

* **Function Description**

  The purpose of this interface is: only subscribe to the monitoring points under a monitoring point group under the box, and the preconditions before the signalr real-time data push event is triggered.

   **NOTE：**The interface needs to be called again every time the box goes online, and it is called according to [the state attribute pushed by the box state change](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjCwKXsmrLO1KxUIV0Z/http-document-1/data-push/untitled-4%20)

* **Request Address \(pick one of two\)**

  **Old Version：**

   **URL:**`[apiBaseUrl]dmon/group/{gid}/start/only`

   **New Version：**

   **URL:**`[Host Server]/api/dmon/group/{gid}/start/only`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | gid | string | Monitoring point group uid |

* **Request Mode**

   `POST`

* **Header**

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
  | 429 | Access interface frequency is too fast |

