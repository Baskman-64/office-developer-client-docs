---
title: "BITOR Function"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251400
 
ms.localizationpriority: medium
ms.assetid: 1d0954c5-b2cb-6c5d-62b3-a68011cf0c85
description: "Returns a 16-bit binary number in which each bit is set to 1 if the corresponding bit in either binary number1 or binary number2 is 1. The bit is set to 0 only if the corresponding bit is 0 in both binary number1 and binary number2."
---

# BITOR Function

Returns a 16-bit binary number in which each bit is set to 1 if the corresponding bit in either *binary number1* or *binary number2* is 1. The bit is set to 0 only if the corresponding bit is 0 in both *binary number1* and *binary number2*.
  
## Syntax

BITOR(***binary number1***, ***binary number2*** )
  
### Parameters

|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| *binary number1* <br/> |Required  <br/> |**Numeric** <br/> |The first 16-bit binary number. |
| *binary number2* <br/> |Required  <br/> |**Numeric** <br/> |The second 16-bit binary number. |

### Return value

16-bit Binary
  
## Example

BITOR(12,6)
  
Returns 14. The 12 = 0...01100. The 6 = 0...00110. Therefore, BITOR(12,6) = 0...01110.
