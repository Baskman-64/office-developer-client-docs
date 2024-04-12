---
title: "ASIN Function"
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251395
 
ms.localizationpriority: medium
ms.assetid: 7d917be4-65b1-002f-48cc-6d81916a1157
description: "Returns the arcsine of a number, for example, the angle whose sine is number."
---

# ASIN Function

Returns the arcsine of a number, for example, the angle whose sine is *number*.
  
## Syntax

ASIN(***number*** )
  
### Parameters

|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| *number* <br/> |Required  <br/> |**Numeric** <br/> |The sine of the angle. |

## Remarks

The input value must be in the range -1 <=  *number*  <= 1, or a #NUM! error is returned. The resulting angle is in the range -PI/2 <= *angle* <= PI/2 radians (-90 <= *angle* <= 90 degrees).
  
## Example

ASIN(1)
  
Returns 90 deg
  