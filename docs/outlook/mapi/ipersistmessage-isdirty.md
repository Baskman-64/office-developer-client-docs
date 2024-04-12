---
title: "IPersistMessageIsDirty"
 
 
manager: lindalu
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IPersistMessage.IsDirty
api_type:
- COM
ms.assetid: 57f688db-3a1c-49ff-a15a-8508bda5de68
---

# IPersistMessage::IsDirty

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Checks the form for changes that were made since the last save.
  
```cpp
HRESULT IsDirty( void );
```

## Parameters

None
  
## Return value

S_OK 
  
> The form has changes that were made since it was last saved.
    
S_FALSE 
  
> The form does not have changes that were made since it was last saved.
    
## Remarks

Form viewers call the **IPersistMessage::IsDirty** method to determine whether the message has unsaved data. 
  
## See also



[IPersistMessage : IUnknown](ipersistmessageiunknown.md)

