---
title: "FlipY Cell (Shape Transform Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251198
 
ms.localizationpriority: medium
ms.assetid: 062022ff-e243-2540-becd-d9b969ce83ce
description: "Indicates whether the shape has been flipped vertically."
---

# FlipY Cell (Shape Transform Section)

Indicates whether the shape has been flipped vertically.
  
|**Value**|**Description**|
|:-----|:-----|
| TRUE  <br/> | The shape has been flipped vertically. |
| FALSE  <br/> | The shape has not been flipped vertically. |
   
## Remarks

To get a reference to the FlipY cell by name from another formula, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
| **Cell name:**  <br/> | FlipY  <br/> |
   
To get a reference to the FlipY cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
| **Section index:**  <br/> |**visSectionObject** <br/> |
| **Row index:**  <br/> |**visRowXFormOut** <br/> |
| **Cell index:**  <br/> |**visXFormFlipY** <br/> |
   

