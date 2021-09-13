# Interface Return Code

* The interface return code is 200, which means the call was successful.
* The interface returns 401, the accessToken obtained from the login interface has expired, and the validity period of the accessToken is 2 hours. Please log in to the interface again according to the refresh\_token adjustment, refresh the access\_token and retry the interface. The refresh\_token is valid for 30 days.
* The interface returns 404, no special instructions, please check whether the url of the interface is filled in correctly, check whether the request method of the interface is correct, if it is to add a box interface, check whether the box serial number is correct
* The interface returns 414, 415, please check whether the format of the interface body is correct, and whether the request method of the interface is correct.
* The interface returns 400, please obtain the error code of X-FBox-Code in the Headers information returned by HTTP and combine it with [Appendix III](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/appendix/untitled-2).
* Return the X-FBox-Code under Headers to 9998, please check whether the FlexManager account that obtained the token can operate on the box.
* Return X-FBox-Code under Headers is 9999, Body format is set \[{},{}\].
* Return X-FBox-Code under Headers is 20008, no monitoring point is found under the box.
* Return the X-FBox-Code under Headers to 20009, and the monitoring point has no write permission.
* Return the X-FBox-Code under Headers to 10050, and the devAlias ​​parameter of the newly added monitoring point needs to fill in the driver's alias.

