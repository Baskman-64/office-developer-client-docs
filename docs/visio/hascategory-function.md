---
title: "HASCATEGORY Function"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
 
ms.localizationpriority: medium
ms.assetid: ed3c997b-0a58-0432-c468-a24614b67f2e
description: "Returns TRUE if the specified string is found in the shape's category list."
---

# HASCATEGORY Function

Returns TRUE if the specified string is found in the shape's category list.
  
## Version Information

Version Added: Visio 2010
  
## Syntax

HASCATEGORY(***category*** )
  
### Parameters

|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| *category* <br/> |Required  <br/> |**String** <br/> |The category to search for. |

### Return value

 **Boolean**
  
## Remarks

 *Categories*  are user-defined strings that you can use to categorize shapes. You can define categories in the User.msvShapeCategories cell in the ShapeSheet for a shape. You can define multiple categories for a shape by separating the categories with semi-colons.
  