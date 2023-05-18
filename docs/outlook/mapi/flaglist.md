---
title: "FLAGLIST"
description: Describes FLAGLIST and provides syntax, members, and additional remarks.
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.FLAGLIST
api_type:
- COM
ms.assetid: b4c0655c-1a3a-4f89-a977-0431db596512
---

# FLAGLIST

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains a list of flags used to indicate the status of address entries during the name resolution process.
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapidefs.h  <br/> |
   
```cpp
typedef struct
{
  ULONG cFlags;
  ULONG ulFlags[MAPI_DIM];
} FlagList, FAR * LPFlagList;

```

## Members

 **cFlags**
  
> Count of MAPI-defined flags in the list.
    
 **ulFlags**
  
> An array of flags that provides the status of the name resolution operation for a recipient. The following flags can be set:
    
MAPI_AMBIGUOUS 
  
> The recipient has been resolved, but not to a unique entry identifier. Other address book containers should not try to resolve this recipient. 
    
MAPI_RESOLVED 
  
> The recipient has been resolved to a unique entry identifier. Other address book containers should not try to resolve this recipient. 
    
MAPI_UNRESOLVED 
  
> The entry has not been resolved. Other address book containers should try to resolve this recipient.
    
## Remarks

The **FLAGLIST** structure is used as a parameter to [IABContainer::ResolveNames](iabcontainer-resolvenames.md). Each of the recipients to be resolved is included in an [ADRLIST](adrlist.md) structure. As the address book container attempts to resolve each recipient, it sets the appropriate flag in the corresponding entry in the **FLAGLIST** structure. All of the entries in the **FLAGLIST** structure are in the same order as the entries in the **ADRLIST** structure. This makes it easy to associate a flag setting with a recipient. 
  
## See also



[ADRLIST](adrlist.md)
  
[IABContainer::ResolveNames](iabcontainer-resolvenames.md)


[MAPI Structures](mapi-structures.md)

