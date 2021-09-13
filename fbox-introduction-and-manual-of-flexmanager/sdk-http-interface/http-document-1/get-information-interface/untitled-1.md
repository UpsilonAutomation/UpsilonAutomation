# Get Geographic Location

* **Function Description**

  This interface is used by the user to obtain the geographic location of the box. \(Only the boxes that have been automatically positioned and reported their geographic location can use this interface to query, and the box will upload the geographic location when it is online\)

* **Request Address \(pick one of two\)**

   **Old Version：**

   **URL:**`[App Server]/api/client/v2/box/location`

   **New Version**

   **URL:**`[Host Server]/api/client/v2/box/location`

* **Address Paramter Description**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | APP Server | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Request Mode**

   `POST`

* **Headers**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |
  | X-FBox-ClientId | string | [See appendix I](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj96b3PNyYjsgMj5D8Y/http-document-1/appendix/untitled) |

* **Body**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | ids | List | Box boxId collection |

* **Successful Response**  
   **Returns the geographic location entity object**

  | Parameter Name | Type | Parameter Description |
  | :--- | :--- | :--- |
  | useLongitude | double | Longitude for manual positioning |
  | useLatitude | double | Latitude of manual positioning |
  | radius | int | Longitude radius |
  | address | string | Detailed address |
  | boxNo | string | Box number |
  | boxId | string | Box Id |
  | longitude | double | Longitude for automatic positioning |
  | latitude | double | Latitude for automatic positioning |
  | locationFetchType | int | Location acquisition type |

* **Return State Code**

  | Parameter Name | Parameter Description |
  | :--- | :--- |
  | 401 | AccessToken expired |
  | 500 | Interface implementation error |

