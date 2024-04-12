---
title: "FBadEntryList"
description: "FBadEntryList validates a list of MAPI entry identifiers. This article describes its syntax, parameters, return value, and remarks."
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- FBadEntryList
api_type:
- HeaderDef
ms.assetid: 270c47c3-ae68-4995-b304-27f861b350d6
---

# FBadEntryList

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Validates a list of MAPI entry identifiers. 
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapival.h  <br/> |
|Implemented by:  <br/> |MAPI  <br/> |
|Called by:  <br/> |Service providers  <br/> |
   
```cpp
BOOL FBadEntryList(
  LPENTRYLIST lpEntryList
);
```

## Parameters

 _lpEntryList_
  
> [in] Pointer to an [ENTRYLIST](entrylist.md) structure that contains an array of entry identifiers to be validated. 
    
## Return value

TRUE 
  
> One or more of the listed entry identifiers are invalid. 
    
FALSE 
  
> All of the listed entry identifiers are valid.
    
## Remarks

The **FBadEntryList** function determines if the entry identifier list has been correctly generated. An example of an invalid identifier is one for which memory has been incorrectly allocated or an identifier of an incorrect size. 
  

