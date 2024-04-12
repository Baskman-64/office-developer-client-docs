---
title: "SEGMENTCOUNT Function"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
 
ms.localizationpriority: medium
ms.assetid: 792ec0e4-4a48-136b-904c-fe269e355070
description: "Returns the number of line segments that make up the path."
---

# SEGMENTCOUNT Function

Returns the number of line segments that make up the path.
  
## Syntax

SEGMENTCOUNT(***pathRef***)
  
### Parameters

|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| *pathRef* <br/> |Required  <br/> |**Integer** <br/> |The Geometry section that represents the path, specified by a reference to Path cell (for example, Geometry1.Path). |

### Return value

Integer
  
## Remarks

Line jumps are not included in the total number of segments returned.
  