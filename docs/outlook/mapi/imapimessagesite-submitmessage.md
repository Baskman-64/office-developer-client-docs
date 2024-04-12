---
title: "IMAPIMessageSiteSubmitMessage"
description: "Describes the syntax, parameters, and return value of IMAPIMessageSiteSubmitMessage, which requests that the current message be queued for delivery."
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IMAPIMessageSite.SubmitMessage
api_type:
- COM
ms.assetid: 6b14c383-8bc6-4e86-bd92-0500272af40d
---

# IMAPIMessageSite::SubmitMessage

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Requests that the current message be queued for delivery.
  
```cpp
HRESULT SubmitMessage(
  ULONG ulFlags
);
```

## Parameters

 _ulFlags_
  
> [in] A bitmask of flags that controls how a message is submitted. The following flag can be set:
    
FORCE_SUBMIT 
  
> MAPI should submit the message even if it might not be sent immediately.
    
## Return value

S_OK 
  
> The call succeeded and has returned the expected value or values.
    
## Remarks

Form objects call the **IMAPIMessageSite::SubmitMessage** method to request that a message be queued for delivery. The message site should call the [IPersistMessage::HandsOffMessage](ipersistmessage-handsoffmessage.md) method before submitting the message. The message does not need to have been previously saved, because **SubmitMessage** should cause the message to be saved if the message has been modified. After the return of **SubmitMessage**, the form must check for a current message and then dismiss itself if none exists. 
  
For a list of interfaces related to form servers, see [MAPI Form Interfaces](mapi-form-interfaces.md).
  
## MFCMAPI reference

For MFCMAPI sample code, see the following table.
  
|**File**|**Function**|**Comment**|
|:-----|:-----|:-----|
|MyMAPIFormViewer.cpp  <br/> |CMyMAPIFormViewer::SubmitMessage  <br/> |MFCMAPI uses the **IMAPIMessageSite::SubmitMessage** method to save the message. First, it calls the **IPersistMessage::HandsOffMessage** method, and then it calls **SubmitMessage**. |
   
## See also



[IPersistMessage::HandsOffMessage](ipersistmessage-handsoffmessage.md)
  
[IMAPIMessageSite : IUnknown](imapimessagesiteiunknown.md)


[MFCMAPI as a Code Sample](mfcmapi-as-a-code-sample.md)
  
[MAPI Form Interfaces](mapi-form-interfaces.md)

