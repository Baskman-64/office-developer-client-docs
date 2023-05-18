---
title: "PidTagDeltaX Canonical Property"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagDeltaX
api_type:
- HeaderDef
ms.assetid: 9bbe996b-1cfc-46d7-bb0a-291c760500ef
description: "Contains the width of a dialog box control in standard Windows dialog units. This is one of the properties that determine the position and size the dialog box."
---

# PidTagDeltaX Canonical Property

**Applies to**: Outlook 2013 | Outlook 2016
  
Contains the width of a dialog box control in standard Windows dialog units.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |PR_DELTAX  <br/> |
|Identifier:  <br/> |0x3F03  <br/> |
|Data type:  <br/> |PT_LONG  <br/> |
|Area:  <br/> |MAPI display table  <br/> |

## Remarks

The **PR_XPOS** ([PidTagXCoordinate](pidtagxcoordinate-canonical-property.md)), **PR_YPOS** ([PidTagYCoordinate](pidtagycoordinate-canonical-property.md)), **PR_DELTAY** ([PidTagDeltaY](pidtagdeltay-canonical-property.md)) properties , and this property control the position and size the dialog box control.
  
## Related resources

### Header files

Mapidefs.h
  
> Provides data type definitions.

Mapitags.h
  
> Contains definitions of properties listed as alternate names.

## See also

[MAPI Properties](mapi-properties.md)  
[MAPI Canonical Properties](mapi-canonical-properties.md)  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)
