---
title: "FtMulDwDw"
description: Describes FtMulDwDw and provides syntax, parameters, and return value.
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.FtMulDwDw
api_type:
- COM
ms.assetid: 8c1a342c-d7ae-4e26-b327-a63cdd3c3ee6
---

# FtMulDwDw

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Multiplies one unsigned 32-bit integer by another.
  
|Property|Value|
|:-----|:-----|
|Header file:  <br/> |Mapiutil.h  <br/> |
|Implemented by:  <br/> |MAPI  <br/> |
|Called by:  <br/> |Client applications and service providers  <br/> |
   
```cpp
FILETIME FtMulDwDw(
  DWORD Multiplicand,
  DWORD Multiplier
);
```

## Parameters

 _Multiplicand_
  
> [in] A double word that contains the unsigned 32-bit integer to be multiplied by the value in the _Multiplier_ parameter. 
    
 _Multiplier_
  
> [in] A double word that contains the unsigned 32-bit integer multiplier.
    
## Return value

The **FtMulDwDw** function returns a [FILETIME](filetime.md) structure that contains the product of the two integers. The two input parameters remain unchanged. 
  

