---
title: "IContabAdminRemoveStore"
 
 
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IContabAdmin.RemoveStore
api_type:
- COM
ms.assetid: 2a5fcf5c-8a5a-4774-b8c9-1ac1ff27947d
---

# IContabAdmin::RemoveStore

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Removes the Contact Address Book (CAB) specified by the given entry ID from the address book hierarchy.
  
```cpp
HRESULT RemoveStore(
ULONG cbEntryID, 
LPENTRYID lpEntryID
);
```

## Parameters

 _cbEntryID_
  
> [in] The byte count in the entry identifier pointed to by the  _lpEntryID_ parameter. 
    
 _lpEntryID_
  
> [in] A pointer to the entry identifier of the object to open.
    

