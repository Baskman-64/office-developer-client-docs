---
title: "DoubleStrikethrough Cell (Character Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm1033762
 
ms.localizationpriority: medium
ms.assetid: c48a77e1-ea3c-7a6d-8c05-f9e0cb434cda

description: "Determines whether text is formatted as double strikethrough."
---

# DoubleStrikethrough Cell (Character Section)

Determines whether text is formatted as double strikethrough.
  
## Remarks

To get a reference to the DoubleStrikethrough cell by name from another formula, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
| **Cell name:**  <br/> | Char.DoubleStrikethrough[  *i*  ]            where  *i*  = <1>, 2, 3... |
   
To get a reference to the DoubleStrikethrough cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
| **Section index:**  <br/> |**visSectionCharacter** <br/> |
| **Row index:**  <br/> |**visRowCharacter** +  *i*            where  *i*  = 0, 1, 2... |
| **Cell index:**  <br/> |**visCharacterDoubleStrikethrough** <br/> |
   

