---
title: "MAPIOFFLINE_CREATEINFO"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
ms.assetid: 539aa31d-7dec-4dbb-93f7-fa060c43565a
description: "The MAPIOFFLINE_CREATEINFO structure is used with HrCreateOfflineObj."
---

# MAPIOFFLINE_CREATEINFO

**Applies to**: Outlook 2013 | Outlook 2016
  
This structure is used with [HrCreateOfflineObj](hrcreateofflineobj.md).
  
```cpp
typedef struct
{
  ULONG      ulSize;
  ULONG      ulCreateFlags;
  LPCWSTR      pwszProfileName;
  ULONG      ulCapabilities;
  const GUID*      pGUID;
  const GUID*      pInstance;
  IMAPIOfflineMgr*    pParent;
  IUnknown*      pMAPISupport;
  MAPIOFFLINE_AGGREGATEINFO*  pAggregateInfo;
  MAPIOFFLINE_CONNECTINFO*  pConnectInfo;
} MAPIOFFLINE_CREATEINFO;
```

## Members

 **ulSize**
  
> The size of structure.

 **ulCreateFlags**
  
> It must be 0.

 **pwszProfileName**
  
> The name of the profile.

 **ulCapabilities**
  
> A bit mask of the following capability flags.

|Value |Description |
|:-----|:-----|
|MAPIOFFLINE_CAPABILITY_OFFLINE  <br/> |The offline object is capable of going offline. |
|MAPIOFFLINE_CAPABILITY_ONLINE  <br/> |The offline object is capable of going online. |

 **pGUID**
  
> Pointer to a GUID that is used to uniquely identify this type of offline object from other offline objects. GUID_GlobalState refers to the global offline object that objects can use as a parent object.

 **pInstance**
  
> Pointer to GUID that uniquely identifies this offline object. It is used to disambiguate this offline objects from other objects.

 **pParent**
  
> Pointer to offline object that is the parent of this offline object and whose changes this offline object will inherit.

 **pMAPISupport**
  
> Identifies the MAPI support object that that will use this offline object. For example, if this offline object is used to keep track of a store's offline and online state, then this is the stores support object. However, if this is an offline object for an object with no support object then it can be NULL.

 **pAggregateInfo**
  
> A pointer to a MAPIOFFLINE_AGGREGATEINFO structure. For more information, see [MAPIOFFLINE_AGGREGATEINFO](mapioffline_aggregateinfo.md).

 **pConnectInfo**
  
> Must be null.

## See also

[HrCreateOfflineObj](hrcreateofflineobj.md)
[MAPIOFFLINE_AGGREGATEINFO](mapioffline_aggregateinfo.md)
