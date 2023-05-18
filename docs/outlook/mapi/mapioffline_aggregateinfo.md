---
title: "MAPIOFFLINE_AGGREGATEINFO"
 
 
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
ms.assetid: 2e502d28-ae09-49d9-a35a-5d77acdcd6f4
---

# MAPIOFFLINE_AGGREGATEINFO

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
The structure is used with [HrCreateOfflineObj](hrcreateofflineobj.md). 
  
```cpp
typedef struct
{
  ULONG            ulSize;
  IUnknown*          pOuterObj;
  IUnknown*          pRefTrackRoot;
} MAPIOFFLINE_AGGREGATEINFO;
```

## Members

 **ulSize**
  
> The size of the structure.
    
 **pOuterObj**
  
> A pointer to the IUnknown object onto which this object is being aggregated. This allows any QueryInterface calls to pass through to the created object.
    
 **pRefTrackRoot**
  
> Must be NULL.
    
## See also



[HrCreateOfflineObj](hrcreateofflineobj.md)
  
[MAPIOFFLINE_CREATEINFO](mapioffline_createinfo.md)

