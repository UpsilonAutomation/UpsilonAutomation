# Login Interface Exception Handling

1. Please check the URl correctly
2. The interface request method is Post
3. The format of the login interface and the re-login interface Body is: application/x-www-form-urlencoded, other interface request formats are application/json format, please pay attention.
4. username and password: the account and password used to log in to FlexManager, please register by yourself. Registered address [fbox360.com](http://fbox360.com/)
5.  Scope: fixed value, please fill in`openid offline_access fbox email profile`
6. Grant\_type: fixed value, please fill in`password`
7. client\_Id and client\_secret are the developer account and password. Please contact the sales application after the call, the login interface returns 400

* The error\_description in the returned body prompts "invalid\_username\_or\_password", please check whether the username and password are correct\(login to [fbox360.com](http://fbox360.com/) to verify\)
* Return the error message "invalid\_client" in the body, check whether there are more spaces before and after client\_Id and client\_secret
* Return the error message "unsupported\_grant\_type" in the body, check whether grant\_type is:`password`
* Return the error message "invalid\_scope" in the body, check whether grant\_type is:`openid offline_access fbox email profile`

After the call, the login interface returns 404, please verify the correct URL  


