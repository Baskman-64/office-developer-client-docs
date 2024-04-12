---
title: "LockDelete Cell (Protection Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251219
 
ms.localizationpriority: medium
ms.assetid: 596c62b7-8d42-1854-d709-592db09a6a84
description: "Locks the shape so that it cannot be deleted."
---

# LockDelete Cell (Protection Section)

Locks the shape so that it cannot be deleted.
  
|**Value**|**Description**|
|:-----|:-----|
| TRUE  <br/> | Shape cannot be deleted  <br/> |
| FALSE  <br/> | Shape can be deleted. |
   
## Remarks

To get a reference to the LockDelete cell by name from another formula, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
| **Cell name:**  <br/> | LockDelete  <br/> |
   
To get a reference to the LockDelete cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
| **Section index:**  <br/> |**visSectionObject** <br/> |
| **Row index:**  <br/> |**visRowLock** <br/> |
| **Cell index:**  <br/> |**visLockDelete** <br/> |
   

