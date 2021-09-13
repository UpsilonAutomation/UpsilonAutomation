# New Alarm Groups

* **Function Description**

   The interface is used for users to new add alarm groups. 

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL:**`[apiBaseUrl]v2/alarm/group`

   **New Version：**

   **URL:**`[Host Server]/api/v2/alarm/group`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Request Mode**

   `PUT`

* **Headers**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | boxId | string | FBox id |
  | name | string | Alarm group name  |
  | memo | string | Alarm group remark |
  | cuids | list | Alarm contact id collection \(if there is no alarm contact, pass an empty array\) |

* **Successful Response**

   `NULL`

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 404 | Name conflict |
  | 409 | Alarm contact does not exist |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
  | 500 | The parameter is wrong |

* \*\*\*\*[**Postman Sample as the below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/AddAlarmGroup.png)\*\*\*\*

![](../../../../../.gitbook/assets/image%20%2824%29.png)

* \*\*\*\*[**The use case is as below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/AddAlarmGroup.gif)\*\*\*\*

![](../../../../../.gitbook/assets/image%20%2827%29.png)

