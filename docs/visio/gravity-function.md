---
title: "GRAVITY Function"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251433
 
ms.localizationpriority: medium
ms.assetid: db80f147-71a0-0b23-bc7e-fe1915dfdd21
description: "Calculates a text block's correct angle of rotation for the indicated shape rotation to prevent the text from turning upside down."
---

# GRAVITY Function

Calculates a text block's correct angle of rotation for the indicated shape rotation to prevent the text from turning upside down.
  
## Syntax

GRAVITY(***angle***,[ ***limit1*** ],[ ***limit2*** ])
  
### Parameters

|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| *angle* <br/> |Required  <br/> |**String** <br/> | The shape's angle. |
| *limit1* <br/> |Optional  <br/> |**String** <br/> |First limit of rotation. Default is 90 degrees. |
| *limit2* <br/> |Optional  <br/> |**String** <br/> |Second limit of rotation. Default is 270 degrees. |

### Return value

String
  
## Remarks

The GRAVITY function is usually used in the TxtAngle cell.
  
The value returned is 180 degrees if *angle* is between the values specified by *limit1* and *limit2*; otherwise the value returned is 0 degrees.
  
All of the arguments are automatically normalized between 0 and 360 degrees by the function. If an argument does not specify units, radians are assumed.
  
## Example 1

GRAVITY(Angle)
  
Returns 180 degrees if  *angle*  is between 90 and 270 degrees; otherwise, returns 0 degrees.
  
## Example 2

GRAVITY(2)
  
Returns 180 degrees, because 2 radians is between 90 and 270 degrees.
  
## Example 3

GRAVITY(100 deg, 110 deg, 290 deg)
  
Returns 0 degrees.
  
## Example 4

GRAVITY(100 deg, 290 deg, 110 deg)
  
Returns 0 degrees.
  