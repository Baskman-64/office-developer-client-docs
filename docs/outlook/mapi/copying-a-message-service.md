---
title: "Copying a Message Service"
manager: lindalu
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
api_type:
- COM
ms.assetid: 01e8ad76-973a-42fa-96aa-f41aabc12b4f
 
 
---

# Copying a Message Service

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
 **To copy a message service to a profile**
  
- Call [IMsgServiceAdmin::CopyMsgService](imsgserviceadmin-copymsgservice.md).
    
When a message service is copied, the new instance of the service is configured in exactly the same way as the original. Sometimes **CopyMsgService** returns the error MAPI_E_ACCESS_DENIED. The most common cause of this error return is a message service that does not allow itself to be duplicated. 
  

