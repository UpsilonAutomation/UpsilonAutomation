# How to obtain historical data?

Need to [create a new historical entry](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/historical-record-interface/untitled-2), and then actively call to [obtain historical data](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/historical-record-interface/untitled-5) acquisition.

The maximum limit of interface parameters is 1000, and 500 is recommended. Time stamp with begin and end in milliseconds \(utc\)

Note After the box is offline, the data will be stored locally in the box, and the cache of the box itself is limited. The more the entries, the shorter the storage time. After the space is full, no more collection. After the box is online, the data will be uploaded one by one

The historical data collected by the box cannot be obtained immediately by adjusting the interface. At present, the historical data reported by the box needs to meet 20 minutes or meet 100 data collections. The collection cycle is configured on the client

The historical data is stored in the server for 3 months

After deleting the history entry, the history data will be cleared  


