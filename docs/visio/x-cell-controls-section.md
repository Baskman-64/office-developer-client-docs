---
title: "X Cell (Controls Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251281
 
ms.localizationpriority: medium
ms.assetid: b7aea554-f491-6a9a-4d07-feeab739a9df

description: "Represents the x -coordinate that indicates the location of a shape's control handle in local coordinates."
---

# X Cell (Controls Section)

Represents the  *x*  -coordinate that indicates the location of a shape's control handle in local coordinates. 
  
## Remarks

To get a reference to the X cell by name from another formula, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
| **Cell name:**  <br/> | Controls.  *name*  .X where Controls.  *name*  is the name of the controls row. |
   
To get a reference to the X cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
| **Section index:**  <br/> |**visSectionControls** <br/> |
| **Row index:**  <br/> |**visRowControl** +  *i*            where  *i*  = 0, 1, 2... |
| **Cell index:**  <br/> |**visCtlX** <br/> |
   

