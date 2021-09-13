# Get Single FBox

* **Interface Function**

   Get all FBox groups under the current user name, and related parameters of FBox under the group

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL：**`[App Server]/api/client/box/reg/boxno/{boxNo}`

   **New Version：**

   **URL：**`[Host Server]/api/client/box/reg/boxno/{boxNo}`

* **Address Parameter Description**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | App Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |
  | boxNo | string | Box serial number |

* **Request Mode**

   `GET`

* **Headers**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

   `NULL`

* **Successful Response**  
   **Returns the boxReg of a single box**

  | Parameter Name |  | Type | Parameter Description |
  | :--- | :--- | :--- | :--- |
  | id |  | string | The registration ID associated with the account assigned by the system when the user adds \(shares\) the box |
  | boxUid |  | string | FBox id |
  | alias |  | string | FBox alias |
  | regData |  | string | FBox registration |
  | owned |  | boolean | Is the owner |
  | shared |  | boolean | Whether to be shared |
  | box |  | json object | refer to the below table |

   **boxReg.box Object Attributes：**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | id | string | FBox uid |
  | boxNo | string | FBox serial numer |
  | boxType | string | 0: standard box，1: mini box |
  | cs | json object | apiBaseUrl: The address of the server to which the box is connected. signalrUrl: SignalR address of box data push |
  | devicePrimarySource | int | FBox drives the data source, 0: FBox, 1: server |
  | memo | string | Remark information |
  | net | int | 0: unknown 1: Ethernet 2: GPRS 4: WIFI \(not supported\) 5: 4G mode |
  | mode | int | 1: Transparent transmission, 0: normal |

* **Return Code**

  | Parameter Name | Parameter Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 404 | Box does not exist |

