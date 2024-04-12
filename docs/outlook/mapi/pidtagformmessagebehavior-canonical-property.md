---
title: "PidTagFormMessageBehavior Canonical Property"
description: Outlines the PidTagFormMessageBehavior canonical property, which contains TRUE if a message should be composed in the current folder. 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagFormMessageBehavior
api_type:
- HeaderDef
ms.assetid: 8fd82432-9fd9-49ed-aa52-72109db04dc9
---

# PidTagFormMessageBehavior Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains TRUE if a message should be composed in the current folder. 
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |PR_FORM_MESSAGE_BEHAVIOR  <br/> |
|Identifier:  <br/> |0x330A  <br/> |
|Data type:  <br/> |PT_LONG  <br/> |
|Area:  <br/> |MAPI common  <br/> |
   
## Remarks

A value of FALSE indicates that the message should be composed as any other interpersonal message, that is, in the Outbox folder. 
  
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

