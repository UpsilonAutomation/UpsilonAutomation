# Open FBox All Monitoring Points

* **Function Description**

  The purpose of this interface is to subscribe to all monitoring points under the box, the preconditions before the signalr real-time data push event is triggered

   **NOTE：**The interface needs to be called again every time the box goes online, and it is called according to [the state attribute pushed by the box state change](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjCwKXsmrLO1KxUIV0Z/http-document-1/data-push/untitled-4)

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL:**`[apiBaseUrl]box/{boxId}/dmon/start`

   **New Version：**

   **URL:**`[Host Server]/api/box/{boxId}/dmon/start`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | string | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |

* **请求方式**

   `POST`

* **Header**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

   `NULL`

* **响应成功**

   `NULL`

* **返回码**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | 调用成功 |
  | 401 | accessToken expired |
  | 429 | Access interface frequency is too fast |
  | 421 | 连接signalr传的guid和调用开点接口传的guid不一致 |
  | 500 | 调用开点接口失败，singalr未连接 |

**注意：http可能会因网络等因素调用失败，请求异常后，需要重试该接口。**

