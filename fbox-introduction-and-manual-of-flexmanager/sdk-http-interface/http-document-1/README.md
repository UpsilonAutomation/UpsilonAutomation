# HTTP Document

## **Interface Introduction** <a id="&#x4FEE;&#x6539;&#x65E5;&#x5FD7;"></a>

Operate and read the status of the device 

1. Please [log in](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8c49qqsBH8ibWnzzI/http-document-1/login-interface/untitled) first to get accessToken 

2. Need to [add a box ](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8c49qqsBH8ibWnzzI/http-document-1/untitled/untitled-1)

3. [A monitoring point needs to be added](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8c49qqsBH8ibWnzzI/http-document-1/untitled/untitled-3-1) in the box, and the monitoring point is connected to the register on the plc. The equipment can be controlled by operating the monitoring point 

4. [Get the FBox list](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8c49qqsBH8ibWnzzI/http-document-1/untitled/untitled-4) according to the accessToken call \(get apiBaseUrl and boxNo or boxId\) 

5. According to apiBaseUrl and boxId or boxNo call to [obtain the list of monitoring points](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8c49qqsBH8ibWnzzI/http-document-1/untitled/untitled-3) \(obtain the monitoring point id\) 

6. Call [monitoring point value write](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8c49qqsBH8ibWnzzI/http-document-1/untitled/untitled-5) \(name priority, monitoring point Id can also be used\) 

7. To obtain real-time data, it is recommended to use [SignalR real-time data push](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj8c49qqsBH8ibWnzzI/http-document-1/data-push/untitled-3)

Note: All interfaces in this document do not support cross-domain requests

## **Modify Log** <a id="&#x4FEE;&#x6539;&#x65E5;&#x5FD7;"></a>

<table>
  <thead>
    <tr>
      <th style="text-align:left">Version Number</th>
      <th style="text-align:left">Illustration</th>
      <th style="text-align:left">Date of Writing</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">1.0</td>
      <td style="text-align:left">Preliminary documentation</td>
      <td style="text-align:left">2016.02</td>
    </tr>
    <tr>
      <td style="text-align:left">1.1</td>
      <td style="text-align:left">Document error correction</td>
      <td style="text-align:left">2016.04</td>
    </tr>
    <tr>
      <td style="text-align:left">1.2</td>
      <td style="text-align:left">
        <p>Addition, deletion and modification of new monitoring point entries, addition,
          deletion and modification of alarm entries, and addition, deletion and
          modification of historical entries. V2 interface descriptions, and these
          interfaces support offline editing.</p>
        <p>2.Replace the alarm history record interface.</p>
        <p>3.Newly added driver interface, download driver interface V2, and support
          offline editing.</p>
      </td>
      <td style="text-align:left">2016.12</td>
    </tr>
    <tr>
      <td style="text-align:left">1.2.1</td>
      <td style="text-align:left">Support 2G, 4G box to get address location</td>
      <td style="text-align:left">2017.5</td>
    </tr>
    <tr>
      <td style="text-align:left">1.2.2</td>
      <td style="text-align:left">
        <p>1.Support multi-channel history record.</p>
        <p>2. Remove the previous V1 interface</p>
      </td>
      <td style="text-align:left">2017.7</td>
    </tr>
    <tr>
      <td style="text-align:left">1.2.3</td>
      <td style="text-align:left">Modify the interface of alarm group and alarm contact</td>
      <td style="text-align:left">2018.4</td>
    </tr>
    <tr>
      <td style="text-align:left">1.2.4</td>
      <td style="text-align:left">
        <p>1.Remove and modify the monitoring point grouping</p>
        <p>2.Remove the basic information of FBox</p>
      </td>
      <td style="text-align:left">2020.8.3</td>
    </tr>
    <tr>
      <td style="text-align:left">1.2.5</td>
      <td style="text-align:left">
        <p>1.Added new creation of developer account and developer account call interface</p>
        <p>2.Add new version of the interface address</p>
      </td>
      <td style="text-align:left">2021.1.14</td>
    </tr>
  </tbody>
</table>

