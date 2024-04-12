---
title: "MNLS_IsBadStringPtrW"
description: "Describes the syntax, parameters, return value, and remarks for MNLS_IsBadStringPtrW, which verifies that a pointer to a wide string is valid."
manager: lindalu
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
ms.assetid: 293a0700-b950-4fc2-a2e5-148d6c846384
---

# MNLS_IsBadStringPtrW

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Verifies that a pointer to a wide string is valid.
  
```cpp
BOOL MNLS_IsBadStringPtrW(
  LPCWSTR lpsz,
  UINT ucchMax);
```

## Parameters

 _lpsz_
  
> [in] A pointer to the wide character string.
    
 _ucchMax_
  
> [in] The maximum length of the string in characters including terminator.
    
## Return value

Returns a Boolean that is true if the string is bad.
  
## Remarks

This function wraps [IsBadStringPtr](https://msdn.microsoft.com/library/aa366714%28VS.85%29.aspx). For more information, see [IsBadStringPtr](https://msdn.microsoft.com/library/aa366714%28VS.85%29.aspx).
  

