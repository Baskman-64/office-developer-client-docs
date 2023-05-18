---
title: "IMAPISupportModifyProfile"
 
 
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IMAPISupport.ModifyProfile
api_type:
- COM
ms.assetid: 33bef4ea-d6c0-4455-b95d-4b29edb9c0bc
---

# IMAPISupport::ModifyProfile

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Makes changes to a message store profile section permanent.
  
```cpp
HRESULT ModifyProfile(
ULONG ulFlags
);
```

## Parameters

 _ulFlags_
  
> [in] A bitmask of flags that indicates the type of message store. The following flag can be set:
    
MDB_TEMPORARY 
  
> The message store is temporary and should not be added to the message store table. When MDB_TEMPORARY is set, **ModifyProfile** returns S_OK immediately. 
    
## Return value

S_OK 
  
> The changes to the profile section were successful.
    
## Remarks

The **IMAPISupport::ModifyProfile** method is implemented for message store provider support objects. Message store providers call **ModifyProfile** to prompt MAPI to modify their profile information. 
  
 **ModifyProfile** adds the profile section that is associated with the calling provider to the list of installed message store provider resources. This causes the message store to be listed in the message store table, which is available to clients through the [IMAPISession::GetMsgStoresTable](imapisession-getmsgstorestable.md) method, and to be opened without the display of a dialog box. 
  
If the MDB_TEMPORARY flag is set, MAPI does nothing and the method returns immediately with S_OK.
  
## See also



[IMAPISession::GetMsgStoresTable](imapisession-getmsgstorestable.md)
  
[IMAPISupport : IUnknown](imapisupportiunknown.md)

