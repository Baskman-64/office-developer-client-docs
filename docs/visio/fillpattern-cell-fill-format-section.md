---
title: "FillPattern Cell (Fill Format Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- vis_sdr.chm375
 
ms.localizationpriority: medium
ms.assetid: dac82a4f-4508-541a-e118-7d79df987232
description: "Determines the fill pattern for the shape. To specify a custom fill pattern, use the USE function in this cell."
---

# FillPattern Cell (Fill Format Section)

Determines the fill pattern for the shape. To specify a custom fill pattern, use the USE function in this cell.
  
|**Value**|**Description**|
|:-----|:-----|
|0  <br/> |None (transparent fill). |
|1  <br/> |Solid foreground color. |
|2 - 40  <br/> |Assorted fill patterns that correspond to indexed entries in the **Fill** dialog box. |
   
## Remarks

You can also set this value using the **Fill** dialog box (on the **Home** tab, in the **Shape** group, click **Fill** and then click **Fill Options**).
  
To get a reference to the FillPattern cell by name from another formula, or from a program using the **CellsU** property, use: 
  
||Value |
|:-----|:-----|
|**Cell name:**  <br/> |FillPattern  <br/> |
   
To get a reference to the FillPattern cell by index from a program, use the **CellsSRC** property with the following arguments: 
  
||Value |
|:-----|:-----|
|**Section index:**  <br/> |**visSectionObject** <br/> |
|**Row index:**  <br/> |**visRowFill** <br/> |
|**Cell index:**  <br/> |**visFillPattern** <br/> |
   

