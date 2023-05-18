---
title: "PidTagOriginallyIntendedRecipEntryId Canonical Property"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.PidTagOriginallyIntendedRecipEntryId
api_type:
- COM
ms.assetid: fc288a7a-1927-484e-b860-9cc118672ed2
description: "Contains the entry identifier of the originally intended recipient of an auto-forwarded message. This property corresponds to the X.400 report per-recipient attribute."
---

# PidTagOriginallyIntendedRecipEntryId Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains the entry identifier of the originally intended recipient of an auto-forwarded message.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |PR_ORIGINALLY_INTENDED_RECIP_ENTRYID  <br/> |
|Identifier:  <br/> |0x1012  <br/> |
|Data type:  <br/> |PT_BINARY  <br/> |
|Area:  <br/> |Server  <br/> |
   
## Remarks

This property is one of the address properties for the originally intended message recipient. It must be set by the automatic agent that has forwarded the message.
  
This property corresponds to the X.400 report per-recipient attribute.
  
## Related resources

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

