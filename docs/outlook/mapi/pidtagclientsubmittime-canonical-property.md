---
title: "PidTagClientSubmitTime Canonical Property"
description: Outlines the PidTagClientSubmitTime canonical property, which contains the date and time the message sender submitted a message. 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagClientSubmitTime
api_type:
- HeaderDef
ms.assetid: d46e1063-6421-410d-a445-7477fea42089
---

# PidTagClientSubmitTime Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains the date and time the message sender submitted a message. 
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |PR_CLIENT_SUBMIT_TIME  <br/> |
|Identifier:  <br/> |0x0039  <br/> |
|Data type:  <br/> |PT_SYSTIME  <br/> |
|Area:  <br/> |Message time  <br/> |
   
## Remarks

The store provider sets **PR_CLIENT_SUBMIT_TIME** to the time that the client application called [IMessage::SubmitMessage](imessage-submitmessage.md). 
  
## Related resources

### Protocol specifications

[[MS-OXOMSG]](https://msdn.microsoft.com/library/daa9120f-f325-4afb-a738-28f91049ab3c%28Office.15%29.aspx)
  
> Handles message and attachment objects.
    
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

