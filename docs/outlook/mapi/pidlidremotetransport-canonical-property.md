---
title: "PidLidRemoteTransport Canonical Property"
description: Outlines the PidLidRemoteTransport canonical property, which identifies what account the header item is associated with.
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidLidRemoteTransport
api_type:
- COM
ms.assetid: b3b30d6a-05cd-4dd1-a162-20768f12e680
---

# PidLidRemoteTransport Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Identifies what account the header item is associated with, primarily to implement the POP Leave on Server functionality. 
  
|Property |Value |
|:-----|:-----|
|Associated Properties  <br/> |dispidRemoteXP  <br/> |
|Property set:  <br/> |PSETID_Remote  <br/> |
|Long ID (LID):  <br/> |0x00008F03  <br/> |
|Data type:  <br/> |PT_STRING8  <br/> |
|Area:  <br/> |Remote message  <br/> |
   
## Remarks

This property is relevant only on messages that have a message class of IPM.Remote. Microsoft Outlook keeps a mapping of various accounts that are downloading to a given store in a Folder Associated Information (FAI) message, but it could also keep this information in the registry.
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]] 
  
> Provides property set definitions and references to related Exchange Server protocol specifications.
    
### Header files

Mapidefs.h
  
> Provides data type definitions.
    
## See also



[MAPI Properties](mapi-properties.md)
  
[MAPI Canonical Properties](mapi-canonical-properties.md)
  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)
  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)

