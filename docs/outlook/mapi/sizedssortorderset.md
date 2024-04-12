---
title: "SizedSSortOrderSet"
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.SizedSSortOrderSet
api_type:
- COM
ms.assetid: f0b9c2f4-7011-414d-8e6c-ab22893ef132
description: "Creates a named SSortOrderSet structure that contains a specified number of sort orders for Outlook 2013 or Outlook 2016."
---

# SizedSSortOrderSet

**Applies to**: Outlook 2013 | Outlook 2016 
  
Creates a named [SSortOrderSet](ssortorderset.md) structure that contains a specified number of sort orders. 
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapidefs.h  <br/> |
|Related structure:  <br/> |**SSortOrderSet** <br/> |
   
```cpp
SizedSSortOrderSet (_csort,_name)
```

## Parameters

__csort_
  
> Count of sort orders to be included in the new structure.
    
__name_
  
> Name for the new structure.
    
## Remarks

Use the **SizedSSortOrderSet** macro to create a sort order set with explicit bounds. 
  
To use the new structure that results from the **SizedSSortOrderSet** macro as a pointer to an **SSortOrderSet** structure, perform the following cast: 
  
```cpp
lpSSortOrderSet = (LPSSortOrderSet) &SizedSSortOrderSet;

```

## See also

- [SSortOrderSet](ssortorderset.md)
- [Macros Related to Structures](macros-related-to-structures.md)

