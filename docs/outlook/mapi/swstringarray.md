---
title: "SWStringArray"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.SWStringArray
api_type:
- COM
ms.assetid: c1ae24ad-1bbb-4dee-b414-b5226593b6fa
description: "Contains an array of character strings that are used to describe a property of type PT_MV_UNICODE."
---

# SWStringArray

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains an array of character strings that are used to describe a property of type PT_MV_UNICODE. 
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapidefs.h  <br/> |
   
```cpp
typedef struct _SWStringArray
{
  ULONG cValues;
  LPWSTR FAR *lppszW;
} SWStringArray;

```

## Members

 **cValues**
  
> Count of strings in the array pointed to by the **lppszW** member. 
    
 **lppszW**
  
> Pointer to an array of null-ended Unicode character strings.
    
## Remarks

For more information about PT_MV_UNICODE, see [Property Types](property-types.md).
  
## See also



[SPropValue](spropvalue.md)


[MAPI Structures](mapi-structures.md)

