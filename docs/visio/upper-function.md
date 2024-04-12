---
title: "UPPER Function"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251509
 
ms.localizationpriority: medium
ms.assetid: ef94ee0f-dbb8-a2e1-1805-8a6609830d2a
description: "Returns a string converted to uppercase."
---

# UPPER Function

Returns a string converted to uppercase.
  
## Syntax

UPPER(***expression***)
  
### Parameters

|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| *expression* <br/> |Required  <br/> |**Varies** <br/> | A string, a cell reference, or an expression; the result is converted to a string, which is then converted to uppercase. |

## Remarks

The case conversion is locale-specific, based on the current user settings.
  
## Example

UPPER("mIxEd CAse")
  
Returns "MIXED CASE".
  