# Interface Introduction

**Operate and read the status of the device**

1.Please [log in ](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjDhmJz6g0jBM5EtQay/http-document-1/login-interface/untitled)first to get accessToken  
2.Need to [add a box](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjDhmJz6g0jBM5EtQay/http-document-1/untitled/untitled-1)  
3.[A monitoring point needs to be added in the box](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjDhmJz6g0jBM5EtQay/http-document-1/untitled/untitled-3-1), and the monitoring point is connected to the register on the plc. The equipment can be controlled by operating the monitoring point  
4.[Get the FBox list](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjDhmJz6g0jBM5EtQay/http-document-1/untitled/untitled-4) according to the accessToken call \(get apiBaseUrl and boxNo or boxId\)  
5.According to apiBaseUrl and boxId or boxNo call to [get the list of monitoring points](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjDhmJz6g0jBM5EtQay/http-document-1/untitled/untitled-3) \(obtain the monitoring point id\)  
6.Call [monitoring point value write](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjDhmJz6g0jBM5EtQay/http-document-1/untitled/untitled-5) \(name priority, monitoring point Id can also be used\)  
7. To obtain real-time data, it is recommended to use [SignalR real-time data push](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-MjDhmJz6g0jBM5EtQay/http-document-1/data-push/untitled-3)

**NOTE:**  
All interfaces in this document do not support cross-domain requests

## **Modify Log** <a id="&#x4FEE;&#x6539;&#x65E5;&#x5FD7;"></a>

| Version No. | Description | Edited Date |
| :--- | :--- | :--- |
| 1.0 | Preliminary documentation | 2016.02 |
| 1.1 | Document error correction | 2016.04 |
| 1.2 | 1.Addition, deletion and modification of new monitoring point entries, addition, deletion and modification of alarm entries, and addition, deletion and modification of historical entries. V2 interface descriptions, and these interfaces support offline editing.  2.Replace the alarm history record interface.  3.Newly added driver interface, download driver interface V2, and support offline editing. | 2016.12 |
| 1.2.1 | Support 2G, 4G box to get address location | 2017.5 |
| 1.2.2 | 1.Support multi-channel history record.  2.Remove the previous V1 interface | 2017.7 |
| 1.2.3 | Modify the interface of alarm group and alarm contact | 2018.4 |
| 1.2.4 | 1.Remove and modify the monitoring point grouping 2.Remove the basic information of FBox | 2020.8.3 |
| 1.2.5 | 1.Added new creation of developer account and developer account call interface 2.Add new version of the interface address | 2021.1.14 |

