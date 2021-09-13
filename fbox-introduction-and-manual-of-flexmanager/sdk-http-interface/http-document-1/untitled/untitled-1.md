# New FBox

* **Function Description：**

   This function is used for user to add FBox

  **NOTE：**  
  Can only be added as an owner, and an FBox can only have one owner at the same time

* **Request address:（ pick one of two）**

  **Old version：**

  **URL:**`[App Server]/api/client/box/reg`

  **New version：**

  **URL:**`[Host Server]/api/client/box/reg`

  **Address parameter description**

* | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | App Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | X-FBox-ClientId | string | See [appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |
* **Methos**

  `POST`

* **Headers**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | See [appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | alias | string | FBox alias |
  | boxNo | string | FBox serial number  |
  | boxPassword | string | FBox password |
  | groupId | string | Choose one of FBox group uid and groupName groupName |
  | groupName | string | Choose one of the FBox group uid and groupName, if it does not exist, add a new group |

* **Successful response**

  Return the regId of the FBox \(the return is not a json format, but a string\)



* **Return Code**

  | Parameter Name | Parameter Description |
  | :--- | :--- |
  | 304 | The FBox has been added |
  | 401 | accessToken expired |
  | 404 | FBox does not exist |
  | 406 | FBox has been added by others |
  | 403 | FBox password error |
  | 414 | Invalid box serial number |
  | 417 | Already own the FBox |

* \*\*\*\*[**The use case is as shown in the figure below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/AddBox.gif)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2870%29.png)

