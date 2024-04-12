---
title: "PidTagPstPathHint Canonical Property"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_type:
- COM
ms.assetid: 9cb4af50-3735-4029-a608-a6e7927019dd
description: "Provides the personal storage table (.pst file) name, which the user can edit, for the configuration dialog box."
---

# PidTagPstPathHint Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Provides the personal storage table (.pst file) name, which the user can edit, for the configuration dialog box. 
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |PR_PST_PATH_HINT, PR_PST_PATH_HINT_A, PR_PST_PATH_HINT_W  <br/> |
|Identifier:  <br/> |0x6771  <br/> |
|Data type:  <br/> |PT_STRING8, PT_UNICODE  <br/> |
|Area:  <br/> |Personal storage table (.pst) internal  <br/> |
   
## Remarks

If the **PR_PST_PATH** ([PidTagPstPath](pidtagpstpath-canonical-property.md)) property is used instead, the configuration dialog box will open, but the user will not be allowed to edit the path and many other properties.
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]] 
  
> Provides references to related Exchange Server protocol specifications.
    
### Header files

Mapidefs.h
  
> Provides data type definitions.
    
Mapitags.h
  
> Contains definitions of properties listed as associated properties.
    
## See also



[MAPI Properties](mapi-properties.md)
  
[MAPI Canonical Properties](mapi-canonical-properties.md)
  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)
  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)

