---
title: "LineGradientEnabled Cell (Gradient Properties Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
 
ms.localizationpriority: medium
ms.assetid: 276a661f-d14e-404a-a494-ae36601a8ce3
description: "Determines whether a line gradient is enabled for a line or border of a shape."
---

# LineGradientEnabled Cell (Gradient Properties Section)

Determines whether a line gradient is enabled for a line or border of a shape. 
  
|**Value**|**Description**|
|:-----|:-----|
|TRUE  <br/> |Gradient is displayed on the line or border of a shape. |
|FALSE  <br/> |Gradients are not displayed on the line or border of a shape. |
   
## Remarks

To get a reference to the **LineGradientEnabled** cell by name from another formula, by value of the **N** attribute of a **Cell** element, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
| **Cell name:**  <br/> | LineGradientEnabled  <br/> |
   
To get a reference to the **LineGradientEnabled** cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
| **Section index:**  <br/> |**visSectionObject** <br/> |
| **Row index:**  <br/> |**visRowGradientProperties** <br/> |
| **Cell index:**  <br/> |**visLineGradientEnabled** <br/> |
   

