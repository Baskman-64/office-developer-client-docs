---
title: "E Cell (Geometry Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251761
 
ms.localizationpriority: medium
ms.assetid: bc0154b1-6930-1fe0-655c-05eab2d60230

description: "Contains a nonuniform rational B-spline (NURBS) formula."
---

# E Cell (Geometry Section)

Contains a nonuniform rational B-spline (NURBS) formula.
  
## Remarks

To get a reference to the E cell by name from another formula, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
| **Cell name:**  <br/> | Geometry  *i*  .E  *j*            where  *i*  and  *j*  = <1>, 2, 3... |
   
To get a reference to the E cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
| **Section index:**  <br/> |**visSectionFirstComponent** +  *i*            where  *i*  = 0, 1, 2... |
| **Row index:**  <br/> |**visRowVertex** +  *j*            where  *j*  = 0, 1, 2... |
| **Cell index:**  <br/> |**visNURBSData** <br/> |
   

