---
title: "PidTagMessageSecurityLabel Canonical Property"
description: Outlines the PidTagMessageSecurityLabel canonical property, which contains a security label for a message.
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagMessageSecurityLabel
api_type:
- HeaderDef
ms.assetid: aae41f1b-19bb-40c7-8564-0c87a5a4e47c
---

# PidTagMessageSecurityLabel Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains a security label for a message.
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |PR_MESSAGE_SECURITY_LABEL  <br/> |
|Identifier:  <br/> |0x001E  <br/> |
|Data type:  <br/> |PT_BINARY  <br/> |
|Area:  <br/> |Server  <br/> |
   
## Remarks

This property provides the basis on which the **PR_MESSAGE_TOKEN** ([PidTagMessageToken](pidtagmessagetoken-canonical-property.md)) property protects a message. Its association with the message content is guaranteed by the token.
  
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

