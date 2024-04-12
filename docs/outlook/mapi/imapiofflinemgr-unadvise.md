---
title: "IMAPIOfflineMgrUnadvise"
 
 
manager: lindalu
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IMAPIOfflineMgr.Unadvise
api_type:
- COM
ms.assetid: 250b9137-facb-81a2-41b1-96a57366c04e
---

# IMAPIOfflineMgr::Unadvise


**Applies to**: Outlook 2013 | Outlook 2016
  
Cancels callbacks for an offline object.
  
```cpp
HRESULT COfflineObj::Unadvise( 
      ULONG ulFlags, 
      ULONG ulAdviseToken 
);
```

## Parameters

 _ulFlags_
  
> [in] Flags for canceling callback. Only the value MAPIOFFLINE_UNADVISE_DEFAULT is supported.

 _ulAdviseToken_
  
> [in] An advise token that identifies the callback registration that is to be canceled.

## Return value

S_OK
  
> The call was successful. This call must return S_OK.

## Remarks

Removes the registration for the callback that was associated with _ulAdviseToken_ returned from a prior call to **[IMAPIOfflineMgr::Advise](imapiofflinemgr-advise.md)**. Causes the **IMAPIOfflineMgr** object to release its reference on the **[IMAPIOfflineNotify](imapiofflinenotifyiunknown.md)** object associated with _ulAdviseToken_.
  
## See also

[IMAPIOfflineMgr::Advise](imapiofflinemgr-advise.md)
[MAPI Constants](mapi-constants.md)
