---
title: "CY Function"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82253223
 
ms.localizationpriority: medium
ms.assetid: abb27f90-21b4-08cd-6995-9520fbcebd78
description: "Returns a currency value."
---

# CY Function

Returns a currency value.
  
## Syntax

CY(***value***, ***cyID*** )
  
### Parameters

|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| *value* <br/> |Optional  <br/> |**Number or String** <br/> |A number or a string that includes currency-specific formatting. If not specified, the currency value is formatted according to the currency style in the system's Region and Language settings. |
| *cyID* <br/> |Optional  <br/> |**Number** <br/> |A numeric currency ID or a three-character quoted string for the ISO 4217 abbreviation. |

## Remarks

To specify a different currency, you must include a valid  *cyID*. For a list, see [About currency constants](about-currency-constants.md).
  
If  *value* is incompatible with the designated currency type, or if an invalid argument such as "not a number" is specified, a #VALUE! error is returned. If  _value_ is greater than 922,337,203,685,477.5807 or less than -922,337,203,685,477.5808, a #VALUE! error is returned.
  
For better precision with very large currency values that include fractions of a unit, such as 3.6 trillion, use string arguments for  *value*.
  
Specifying an invalid  *cyID* returns an error.
  
## Example 1

If the user's Region and Language settings specify United States dollars:
  
CY(999998.993)
  
Returns $999,998.99
  
## Example 2

CY(12345678.993, "USD")
  
Returns $12,345,678.99
  
## Example 3

CY(12345678.993, "DEM")
  
Returns 12,345,678.99 DEM
  
## Example 4

CY(12345678.7832, "XXX")
  
Returns 12,345,678.78
  