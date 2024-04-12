---
title: "NoProofing Cell (Miscellaneous Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: overview
 
ms.localizationpriority: medium
ms.assetid: 668f993c-b4d1-4762-9801-c578b17fdafd
description: "Determines whether spelling is automatically corrected and whether spelling errors are displayed for the selected shape. Takes a Boolean value."
---

# NoProofing Cell (Miscellaneous Section)

Determines whether spelling is automatically corrected and whether spelling errors are displayed for the selected shape. Takes a **Boolean** value. 
  
|**Value**|**Description**|
|:-----|:-----|
|TRUE  <br/> |Spelling is not automatically corrected and spelling errors are not displayed for the selected shape. |
|FALSE  <br/> |Spelling is automatically corrected and spelling errors are displayed for the selected shape. |
   
## Remarks

To get a reference to the NoProofing cell by name from another formula or from a program, by using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
|**Cell name:**  <br/> |NoProofing  <br/> |
   
To get a reference to the NoProofing cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
|**Section index:**  <br/> |**visSectionObject** <br/> |
|**Row index:**  <br/> |**visRowMisc** <br/> |
|**Cell index:**  <br/> |**visObjNoProofing** <br/> |
   

