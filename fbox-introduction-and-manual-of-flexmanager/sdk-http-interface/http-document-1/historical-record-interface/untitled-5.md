# Get Historical Record Data

* **Function Description**

   This interface is used for users to obtain historical data \(there is a frequency limit, each IP should not exceed five times a second, if it exceeds a certain frequency, the IP will be blocked by the Ng proxy\)

* **Request Address \(pick one of two\)**

   **Old Version:**

   **URL:**`[hsserver]/v2/hdata/get`

   **New Version:**

   **URL:**`[Host Server]/hs/v2/hdata/get`

* **Address Parameter Description**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | hsserver | string | see [Noun Explaination](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8wlgyy_R51z8IfQDt/http-document-1/login-interface/noun-explain-or-fbox-document) for more details |

* **Request Mode**

   `POST`

* **Header**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | Authorization | string | "Bearer" + accessToken obtained in the login interface |

* **Body**

  | Field Name | Type | Description |
  | :--- | :--- | :--- |
  | type | int | 0: by row \(time 1: entry 1 data, entry 2 data, time 2: entry 1 data, entry 2 data,...\) 1: by column \(entry 1: time 1 data 1, time 2 data 2,. .. Entry 2: Time 1 Data 1, Time 2 Data 2\) |
  | format | int | 0:JSON 1:CSV file download |
  | ids | Array | List of channel IDs under history entries |
  | names | Array | History entry name \(only used for the header of the export function\) |
  | g | int | 0: Raw data 1: Sub-data 2: Hourly data 3: Daily data |
  | begin | dateTime | Start time \(Javascript timestamp, the number of milliseconds from 1970-1-1 to the present\) |
  | end | dateTime | End time \(same as above\) |
  | tr | int | Time condition boundary type \(0: left open, right open 1: left open, right closed 2: left closed, right open 3: left closed, right closed. Left represents the start time, right represents the end time\) |
  | limit | int | The maximum number of data items to be obtained. A negative value means that the limit items are taken forward from the end time, and the end of the return is in the positive order of time. The maximum limit is 1000, 500 is recommended |
  | tz | string | Linux time zone string \(for example: Asia/Shanghai\), specify the time zone of the time in the csv export data |

* **Successful Response**

   
   **NOTE**  
   t represents the unix epoch time, c is the returned data array, followed by the channels 1, 2, 3, 4, 5, 6, and 7. The channels are based on the order of the channels passed in by the user.

* **Return Code**

  | Field Name | Description |
  | :--- | :--- |
  | 200 | Execution succeed |
  | 401 | accessToken expired |
  | 400 | The error message is in the HTTP Header \[X-FBox-Code\], see [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjC0dIK6gMQjbDiItxW/http-document-1/appendix/untitled-2) for details |
  | 404 | Interface does not exist, please check URL |
  | 429 | Access interface frequency is too fast |

* \*\*\*\*[**Postman sample as below**](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/queryhdata.png)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2842%29.png)

* [**The use case is as below** ](https://docs.flexem.net/fbox/zh-cn/tutorials/Images/ApiDocs/AddHistoryData.gif)\*\*\*\*

![](../../../../.gitbook/assets/image%20%2843%29.png)

