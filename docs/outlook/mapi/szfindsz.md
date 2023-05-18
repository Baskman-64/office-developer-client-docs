---
title: "SzFindSz"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.SzFindSz
api_type:
- COM
ms.assetid: f4584569-1246-4ac9-a404-48284e4920d7
description: "Locates the first occurrence of a null-terminated substring in a null-terminated string. Searches in Unicode and DBCS formats are supported."
---

# SzFindSz

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Locates the first occurrence of a null-terminated substring in a null-terminated string. 
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapiutil.h  <br/> |
|Implemented by:  <br/> |MAPI  <br/> |
|Called by:  <br/> |Client applications and service providers  <br/> |
   
```cpp
LPSTR SzFindCh(
  LPCSTR lpsz,
  LPCSTR lpszKey
);
```

## Parameters

 _lpsz_
  
> [in] Pointer to the null-terminated string to be searched. The  _lpsz_ parameter must not exceed 65536 characters. 
    
 _lpszKey_
  
> [in] Pointer to the null-terminated substring to be searched for. The  _lpszKey_ parameter must not exceed 65536 characters. 
    
## Return value

 **SzFindSz** returns a pointer to the first character of the first occurrence of the substring in the string. If the substring does not occur anywhere in the string, if  _lpszKey_ is larger than  _lpsz_, or if either parameter is NULL, a value of NULL is returned. 
  
## Remarks

The **SzFindSz** function searches for an exact match only; it is sensitive to case and diacritical differences. Searches in Unicode and DBCS formats are supported. The length limit on both parameters is in characters, not necessarily bytes. 
  

