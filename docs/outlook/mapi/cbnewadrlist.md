---
title: "CbNewADRLIST"
description: "CbNewADRLIST computes the number of bytes that should be allocated for a new ADRLIST structure that contains a specified number of recipients represented by ADRENTRY structures."
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.CbNewADRLIST
api_type:
- COM
ms.assetid: 9ec1bbaa-7707-4239-9994-21ad1116430b
---

# CbNewADRLIST

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Computes the number of bytes that should be allocated for a new [ADRLIST](adrlist.md) structure that contains a specified number of recipients represented by [ADRENTRY](adrentry.md) structures. 
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapidefs.h  <br/> |
|Related structure:  <br/> |**ADRLIST** <br/> |
   
```cpp
CbNewADRLIST (_centries)
```

## Parameters

 __centries_
  
> Count of **ADRENTRY** structures to be included in the new **ADRLIST** structure. 
    
## See also



[ADRLIST](adrlist.md)
  
[ADRENTRY](adrentry.md)


[Macros Related to Structures](macros-related-to-structures.md)

