---
title: "NoShow Cell (Geometry Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm735
 
ms.localizationpriority: medium
ms.assetid: 831075ff-2875-b598-00bb-eb8481fee57b

description: "Indicates whether a path is displayed on the drawing page."
---

# NoShow Cell (Geometry Section)

Indicates whether a path is displayed on the drawing page.
  
|**Value**|**Description**|
|:-----|:-----|
| TRUE  <br/> | The stroke and fill of the path represented by the section is hidden. |
| FALSE  <br/> | The stroke and fill of the path is shown. |
   
## Remarks

To get a reference to the NoShow cell by name from another formula, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
| **Cell name:**  <br/> | Geometry  *i*  .NoShow            where  *i*  = <1>, 2, 3... |
   
To get a reference to the NoShow cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
| **Section index:**  <br/> |**visSectionFirstComponent** +  *i*            where  *i*  = 0, 1, 2... |
| **Row index:**  <br/> |**visRowComponent** <br/> |
| **Cell index:**  <br/> |**visCompNoShow** <br/> |
   

