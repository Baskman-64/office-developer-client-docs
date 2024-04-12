---
title: "LockHeight Cell (Protection Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- vis_sdr.chm635
 
ms.localizationpriority: medium
ms.assetid: 218b957e-5af6-e53b-1453-a84164ae456e
description: "Locks the height of the shape so that its height remains unchanged when the shape is resized."
---

# LockHeight Cell (Protection Section)

Locks the height of the shape so that its height remains unchanged when the shape is resized.
  
|**Value**|**Description**|
|:-----|:-----|
| TRUE  <br/> | Height is locked. |
| FALSE  <br/> | Height is not locked. |
   
## Remarks

To get a reference to the LockHeight cell by name from another formula, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
| **Cell name:**  <br/> | LockHeight  <br/> |
   
To get a reference to the LockHeight cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
| **Section index:**  <br/> |**visSectionObject** <br/> |
| **Row index:**  <br/> |**visRowLock** <br/> |
| **Cell index:**  <br/> |**visLockHeight** <br/> |
   

