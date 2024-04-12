---
title: "PidLidNonSendableTo Canonical Property"
description: Outlines the PidLidNonSendableTo canonical property, which contains a list of all the unsendable attendees who are also required attendees.
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidLidNonSendableTo
api_type:
- COM
ms.assetid: 90e14969-652b-422a-9b0a-ee99e58bc8d5
---

# PidLidNonSendableTo Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains a list of all the unsendable attendees who are also required attendees.
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |dispidNonSendableTo  <br/> |
|Property set:  <br/> |PSETID_Common  <br/> |
|Long ID (LID):  <br/> |0x00008536  <br/> |
|Data type:  <br/> |PT_UNICODE  <br/> |
|Area:  <br/> |Meetings  <br/> |
   
## Remarks

The value for each attendee is the **PR_DISPLAY_NAME** ([PidTagDisplayName](pidtagdisplayname-canonical-property.md)) property of the attendee's Address Book. Separate entries must be delimited by a semicolon followed by a space. This property is not required.
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]](https://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> Provides property set definitions and references to related Exchange Server protocol specifications.
    
[[MS-OXOCAL]](https://msdn.microsoft.com/library/09861fde-c8e4-4028-9346-e7c214cfdba1%28Office.15%29.aspx)
  
> Specifies the properties and operations for appointment, meeting request, and response messages.
    
### Header files

Mapidefs.h
  
> Provides data type definitions.
    
## See also



[MAPI Properties](mapi-properties.md)
  
[MAPI Canonical Properties](mapi-canonical-properties.md)
  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)
  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)

