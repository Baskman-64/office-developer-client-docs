---
title: "LockGroup Cell (Protection Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251227
 
ms.localizationpriority: medium
ms.assetid: 04b0fa5b-1680-cfe2-6aaf-0502ad196027
description: "Locks a group so that it cannot be ungrouped."
---

# LockGroup Cell (Protection Section)

Locks a group so that it cannot be ungrouped.
  
|**Value**|**Description**|
|:-----|:-----|
|TRUE  <br/> |Group cannot be ungrouped. |
|FALSE  <br/> |Group can be ungrouped. |
   
## Remarks

Setting the LockGroupCell value to TRUE also prevents deletion of any shapes that are members of the group.
  
To get a reference to the LockGroup cell by name from another formula, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
|**Cell name:**  <br/> |LockGroup  <br/> |
   
To get a reference to the LockGroup cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
|**Section index:**  <br/> |**visSectionObject** <br/> |
|**Row index:**  <br/> |**visRowLock** <br/> |
|**Cell index:**  <br/> |**visLockGroup** <br/> |
   

