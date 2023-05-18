---
title: "IFolderSupportGetSupportMask"
 
 
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IFolderSupport.GetSupportMask
api_type:
- COM
ms.assetid: 8d8aaeb7-57d7-ba4c-95d1-a5368cfc4afe
---

# IFolderSupport::GetSupportMask

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Gets information about a folder's support for sharing.
  
```cpp
HRESULT GetSupportMask( 
    DWORD * pdwSupportMask 
); 
```

## Parameters

 _pdwSupportMask_
  
> [out] A bitmask indicating if the folder supports sharing.
    
 **FS_NONE**
  
> Indicates that the folder does not support sharing.
    
 **FS_SUPPORTS_SHARING**
  
> Indicates that the folder supports sharing.
    
## Return value

S_OK 
  
> The call was successful.
    

