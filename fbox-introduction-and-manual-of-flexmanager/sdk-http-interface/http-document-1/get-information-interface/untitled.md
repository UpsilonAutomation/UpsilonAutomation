# Obtain IoT Card Iccid、Imei

* **Function Description**

   This interface can be used to obtain the information of the IoT card

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL:** `[App server]/api/client/v2/box/{boxId}/sim/card`

   **New Version**

   **URL:**`[Host Server]/api/client/v2/box/{boxId}/sim/card`

* **Address Paramter Description**

  | Field Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | App server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |

* **Request Mode**

   `GET`

* **Headers**

  | Field Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   `NULL`

* **Successful Response**

  | Field Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | iccid | string | SIM card serial number |
  | imei | string | International Mobile Subscriber Identity Code |

* **Return Code**

  | Field Name | Parameter Description |
  | :--- | :--- |
  | 200 | Execution success |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/appendix/untitled-2) for details |
  | 404 | The interface does not exist, please check the URL |
  | 429 | Access interface too frequently |

