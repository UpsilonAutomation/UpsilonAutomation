# FBox List Obtaining

* **Interface Function**

​ Get all FBox groups under the current user name, and FBox related parameters under the group.

* **Request Address:（pick one of two）**

  **Old Version：**

   **URL:** `[App Server]/api/client/box/grouped`

  **New Version：**

   **URL:** `[Host Server]/api/client/box/grouped`

* **Address Parameter Description**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | App Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Request Code**

  `GET`

* **Headers**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | Authorization | string | the id in box under boxRegs in [FBox List Obtaining](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/untitled/untitled-4) |
  | X-FBox-ClientId | string | see [Appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj9gNHJSzXO8L7zJd-l/http-document-1/appendix/untitled) |

* **Body**

   `NULL`

* **Return Field**

​ The server FBox group returns an array, and each element {JSON object type} in the array represents a group. The return structure is as follows:

 **Grouping Unit JSON Object Structure**

| Parameter Name | Type | Parameter Description |
| :--- | :--- | :--- |
| id | string | FBox group ID |
| name | string | FBox group name |
| boxRegs | JSON Array | refer to the below table |

**boxRegs JSON Array Element Attributes:**

| Parameter Name | Type | Parameter Description |
| :--- | :--- | :--- |
| id | string | The registration ID associated with the account assigned by the system when the user adds \(shares\) the box |
| alias | string | FBox alias |
| regData | string | FBox registration time |
| owned | boolean | Is the owner |
| shared | boolean | whether to be shared |
| box | json object | refer to the below table |

**boxReg.box Object Attributes：**

| Parameter Name | Type | Parameter Description |
| :--- | :--- | :--- |
| id | string | The Id of the FBox, the BoxId parameter in the interface Url |
| uid | string | The Id of the FBox, the BoxId parameter in the interface Url |
| boxNo | string | FBox serial number |
| boxType | int | 0: standard box, 1: mini box |
| cs | json object | apiBaseUrl: the server address of the box connection, signalrUrl: the SignalR address of the box data push devicePrimarySource |
| devicePrimarySource | int | FBox drives the data source, 0: FBox, 1: server |
| memo | string | remark information |
| net | int | 0: unknown 1: Ethernet 2: GPRS 4: WIFI \(not supported\) 5: 4G |
| mode | int | 1: Transparent transmission, 0: normal |

 **Remark**  
 connectionState \(FBox online status\): 0: Unknown 1: Connected 2: Timed out 3: Disconnected

* **Return Code**

  | Parameter Name | Parameter Description |
  | :--- | :--- |
  | 401 | accessToken expired |
  | 404 | The interface does not exist, please check the URL |
  | 500 | The interface is abnormal or the network is abnormal |

* \*\*\*\*[**The call case is as shown below**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/GetFBoxList.png)\*\*\*\*

![](../../../../.gitbook/assets/image%20%286%29.png)

