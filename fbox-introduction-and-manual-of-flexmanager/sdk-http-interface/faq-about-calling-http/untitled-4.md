# Alarm Data

You need to [add new alarm entries](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/alarm-interface/alarm-record-interface/untitled-1-1), and report after the alarm conditions are met. If the conditions are always met, only the first alarm information will be reported. After the data is restored, the alarm conditions will be reported again. Can listen to [signalr event reception](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/data-push/untitled-2)

The newly added interface reports 400, the X-FBox-Code of Headers is 9999, and the body of the interface is an array

Note Public cloud supports WeChat public account push alarms, only push alarms

The names of the alarm items under the box cannot be the same.

Cannot delete the group with alarm entry under the alarm group  


