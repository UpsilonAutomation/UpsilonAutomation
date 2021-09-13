# How to control device?

1.Log in to the FlexManager software  
2. Add the box and make the box online  
3. Remote download -&gt; configure the drive device corresponding to the PLC  
4. Configure monitoring points \(corresponding to PLC address point table\)  
 Please ask the automation engineer to configure. After completion, you can request to control the device via http

5. Call the interface [write the monitoring point value](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/untitled/untitled-5). The value in the interface is the command to control the equipment, please ask the automation engineer The name and groupname in the interface are the monitoring point name and the monitoring point grouping. You can view the Id in the interface through FlexManager, and you can view it by [obtaining the list of monitoring points](https://app.gitbook.com/@upsilonauto/s/sdk-interface-and-http-interface/~/drafts/-Mj75zBH304KkN9PgZPN/http-document-1/untitled/untitled-3)

**Note: The interface return code is 400, check the X-FBox-Code error code under Headers returned by the interface, and then refer to Appendix III**  
  


