---
title: "PidTagIpmSubtreeEntryId Canonical Property"
description: Outlines the PidTagIpmSubtreeEntryId canonical property, which represents the root of the IPM hierarchy.
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagIpmSubtreeEntryId
api_type:
- HeaderDef
ms.assetid: 5763fc78-5192-4162-be27-4aadc7ed65bc
---

# PidTagIpmSubtreeEntryId Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains the entry identifier of the root of the interpersonal message (IPM) folder subtree in the message store's folder tree. 
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |PR_IPM_SUBTREE_ENTRYID  <br/> |
|Identifier:  <br/> |0x35E0  <br/> |
|Data type:  <br/> |PT_BINARY  <br/> |
|Area:  <br/> |Folder  <br/> |
   
## Remarks

This property represents the root of the IPM hierarchy. IPM clients should not display any folders that are not subfolders of the folder represented by this property.
  
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

