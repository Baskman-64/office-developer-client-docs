---
title: "GOTOPAGE Function"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251432
 
ms.localizationpriority: medium
ms.assetid: b131badf-1656-132e-0aae-eeedb917ba7a
description: "Displays the page that has the name pagename in the currently active window."
---

# GOTOPAGE Function

Displays the page that has the name  *pagename*  in the currently active window.
  
## Syntax

GOTOPAGE(" ***pagename*** ")
  
### Parameters

|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| *pagename* <br/> |Required  <br/> |**String** <br/> |The name of the page to go to. |

## Remarks

If a window is already displaying the page, that window becomes active. If *pagename* does not exist, the application attempts to navigate to https://  *pagename*  /. If Visio is acting as an in-place server, the GOTOPAGE function has no effect.
  
You can use the HYPERLINK function to navigate to any DOS, UNC, or URL path.
  
In earlier versions of Visio products, this function appears as _GOTOPAGE. Visio versions 4.0 and later accept either style.
  