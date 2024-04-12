---
title: "Y Justify Cell (Action Tags Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm1026937
 
ms.localizationpriority: medium
ms.assetid: 27042b62-7623-95d7-7e10-f589d74605c7

description: "The y -offset of the action tag button relative to the point defined by the X and Y cells."
---

# Y Justify Cell (Action Tags Section)

The *y*  -offset of the action tag button relative to the point defined by the X and Y cells.
  
> [!NOTE]
> In previous versions of Microsoft Visio, action tags are called smart tags.
  
|**Value**|**Description**|**Automation constant**|
|:-----|:-----|:-----|
| 0  <br/> | Top justified (the default). |**visSmartTagYJustifyTop** <br/> |
| 1  <br/> | Centered. |**visSmartTagYJustifyMiddle** <br/> |
| 2  <br/> | Bottom justified. |**visSmartTagYJustifyBottom** <br/> |

## Remarks

The X Justify and Y Justify cells determine where the action tag button is placed in relation to the point defined in the X and Y cells.
  
To get a reference to the Y Justify cell by name from another formula, or from a program using the **CellsU** property, use:
  
||Value |
|:-----|:-----|
| **Cell name:**  <br/> | SmartTags. *name* .YJustify where SmartTags. *name* is the name of the action tag row.  <br/> |

To get a reference to the Y Justify cell by index from a program, use the **CellsSRC** property with the following arguments:
  
||Value |
|:-----|:-----|
| **Section index:**  <br/> |**visSectionSmartTag** <br/> |
| **Row index:**  <br/> |**visRowSmartTag** +  *i*            where  *i*  = 0, 1, 2... |
| **Cell index:**  <br/> |**visSmartTagYJustify** <br/> |
