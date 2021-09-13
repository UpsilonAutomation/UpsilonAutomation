# New FBox Grouping

* **Interface Function**

  This interface is used for users to add FBox groups

* **Request address:（ pick one of two）**

  **Old version：**

  **URL:**`[App Server]/api/client/group`

  **New version：**

  **URL:**`[Host Server]/api/client/group`

* **Address parameter description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | App Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Request method**

  `PUT`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | name | string | group name |

* **Return Data：**

   Returns the group id \(groupId\) of the added group, not in JSON format.



* **Return Code**

  | Return Code | Description |
  | :--- | :--- |
  | 200 | Request succeeded |
  | 401 | accessToken expired |
  | 404 | Name is required |
  | 409 | Duplicate name |

* \*\*\*\*[**The use case is as shown in the figure below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/AddBoxGroup.gif)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2863%29.png)

