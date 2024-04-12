---
title: "PlaceFlip Cell (Page Layout Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82253251
 
ms.localizationpriority: medium
ms.assetid: df014b98-cfd5-b6d3-4b8a-b0acb3b94412
description: "Determines how placeable shapes flip and/or rotate on a page when you use the Configure Layout dialog box (on the Design tab, in the Layout group, click Re-Layout Page, and then click More Layout Options)."
---

# PlaceFlip Cell (Page Layout Section)

Determines how placeable shapes flip and/or rotate on a page when you use the **Configure Layout** dialog box (on the **Design** tab, in the **Layout** group, click **Re-Layout Page**, and then click **More Layout Options**).
  
|**Value**|**Description**|**Automation constant**|
|:-----|:-----|:-----|
|&amp;H0  <br/> |Default. Do not flip. |**visLOFlipDefault** <br/> |
|&amp;H1  <br/> |Flip horizontal. |**visLOFlipX** <br/> |
|&amp;H2  <br/> |Flip vertical. |**visLOFlipY** <br/> |
|&amp;H4  <br/> |Flip in 90 degree increments. |**visLOFlipRotate** <br/> |
|&amp;H8  <br/> |Do not flip. |**visLOFlipNone** <br/> |
   
## Remarks

The value in the PlaceFlip cell helps orient a placeable shape toward the next placeable shape it is connected to. It is typically used when laying out drawings that use static glue.
  
To set this behavior for a particular shape, use the ShapePlaceFlip cell in the Shape Layout section.
  
To get a reference to the PlaceFlip cell by name from another formula, or from a program by using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
|**Cell name:**  <br/> |PlaceFlip  <br/> |
   
To get a reference to the PlaceFlip cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
|**Section index:**  <br/> |**visSectionObject** <br/> |
|**Row index:**  <br/> |**visRowPageLayout** <br/> |
|**Cell index:**  <br/> |**visPLOPlaceFlip** <br/> |
   

