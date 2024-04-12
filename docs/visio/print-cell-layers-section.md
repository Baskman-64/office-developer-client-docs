---
title: "Print Cell (Layers Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm825
 
ms.localizationpriority: medium
ms.assetid: 9c76bf02-7269-65bb-2fd2-920243d962ef
description: "Specifies whether shapes belonging to the layer can be printed."
---

# Print Cell (Layers Section)

Specifies whether shapes belonging to the layer can be printed.
  
|**Value**|**Description**|
|:-----|:-----|
|TRUE  <br/> |Shapes can be printed. |
|FALSE  <br/> |Shapes cannot be printed. |
   
## Remarks

You can also set this value by using the **Print** option in the **Layer Properties** dialog box (on the **Home** tab, in the **Editing** group, click **Layers**, and then click **Layer Properties**).
  
To get a reference to the Print cell by name from another formula, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
|**Cell name:**  <br/> |Layers.Print[ *i*  ] where  *i*  = <1>, 2, 3... |
   
To get a reference to the Print cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
|**Section index:**  <br/> |**visSectionLayer** <br/> |
|**Row index:**  <br/> |**visRowLayer** +  *i*  where  *i*  = 0, 1, 2... |
|**Cell index:**  <br/> |**visDocPreviewScope** <br/> |
   

