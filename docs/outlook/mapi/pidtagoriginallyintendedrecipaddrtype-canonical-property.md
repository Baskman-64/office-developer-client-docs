---
title: "PidTagOriginallyIntendedRecipAddrtype Canonical Property"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.PidTagOriginallyIntendedRecipAddrtype
api_type:
- COM
ms.assetid: dcfb6bd5-bff5-4a50-aec7-4bdfdabf7631
description: "Contains the address type of the originally intended recipient of an autoforwarded message. It must be set by the automatic agent that has forwarded the message."
---

# PidTagOriginallyIntendedRecipAddrtype Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains the address type of the originally intended recipient of an autoforwarded message.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |PR_ORIGINALLY_INTENDED_RECIP_ADDRTYPE, PR_ORIGINALLY_INTENDED_RECIP_ADDRTYPE_A, PR_ORIGINALLY_INTENDED_RECIP_ADDRTYPE_W  <br/> |
|Identifier:  <br/> |0x007B  <br/> |
|Data type:  <br/> |PT_STRING8, PT_UNICODE  <br/> |
|Area:  <br/> |Server  <br/> |
   
## Remarks

These properties are one of the address properties for the originally intended message recipient. It must be set by the automatic agent that has forwarded the message.
  
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

