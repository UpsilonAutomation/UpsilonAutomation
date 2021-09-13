# Delete FBox

* **Interface Function**

   This interface is used for users to delete FBox.

   **NOTE：**  
   It can only be deleted by the owner of the FBox. The shareee of the FBox cannot actively delete the FBox. After the FBox owner deletes the FBox, all the shareees will automatically cancel the sharing of the FBox.

* **Request Address:**

   **URL:**`[Host Server]/api/client/v2/box/{boxId}`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | App Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxId | Long | the id in the box under the boxRegs in the interface of [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |

* **Request Mode**

   `DELETE`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

   `NULL`

* **Successful Response**

   `NULL`

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 403 | FBox does not exist |
  | 404 | Not the owner of the FBox |

