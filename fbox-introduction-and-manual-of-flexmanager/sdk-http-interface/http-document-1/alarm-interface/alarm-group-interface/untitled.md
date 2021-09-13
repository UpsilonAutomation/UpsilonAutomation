# Get the List of Alarm Groups

* **Function Description**

   The interface is used for users to get the list of alarm groups.

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL:**`[apiBaseUrl]v2/alarm/group/get`

   **New Version：**

   **URL:**`[Host Server]/api/v2/alarm/group/get`

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
  | boxId | long | FBox的Id |

* **Successful Request**  
   **Return a list of all alarm groups, each group item is a jsonObject**

  | Field Name |  | Type | Description |
  | :--- | :--- | :--- | :--- |
  | uid |  | long | Alarm group uid |
  | name |  | string | Alarm group alias |
  | contactList |  | list | Alarm contact name collection |
  | memo |  | string | Remark information |
  | contacts |  | list | The attribute collection of a single contact is shown in the table below |

   **contactList中单个contacts属性：**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | uid | long | Alarm contact id |
  | name | string | larm contact name |
  | cellphone | string | larm contact mobile |
  | noticeType | int | 1: SMS 2: Voice 3: SMS & Voice |
  | email | string | Alarm contact email |
  | enable | bool | Whether to enable |
  | memo | string | Remark |

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 404 | Interface does not exist, pleas check URL |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [`Appendix III`](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |

