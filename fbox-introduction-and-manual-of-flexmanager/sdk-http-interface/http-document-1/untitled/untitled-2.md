# New Monitoring Point Grouping

* **Function Description**

   This interface is used for user to new add monitoring point grouping.

* **Request address:（ pick one of two）**

  **Old version：**

  **URL:**`[apiBaseUrl]dmon/def/group`

  **New version：**

  **URL:**`[Host Server]/api/dmon/def/group`

\`\`

**Address parameter description**

| Parameter Name | Type | Parameter Description |
| :--- | :--- | :--- |
| apiBaseUrl | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Request Method**

   `PUT`

* **Headers**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | See [appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | name | string | monitoring point group name |
  | boxUid | string | Box Id |

* **Successful response**

  Return the regId of the FBox \(the return is not a json format, but a string\)

  \*\*\*\*

* **Return Code**

  | Status Code | Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 400 | FBox uid  erros |
  | 404 | The interface does not exist, please check the URL |
  | 409 | Duplicate name |
  | 500 | Interface implementation error |

* \*\*\*\*[**The use case is as shown in the figure below:**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/DatamonitoringGroup.gif)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2858%29.png)

