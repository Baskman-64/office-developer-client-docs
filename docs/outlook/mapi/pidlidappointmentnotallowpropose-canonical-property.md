---
title: "PidLidAppointmentNotAllowPropose Canonical Property"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidLidAppointmentNotAllowPropose
api_type:
- COM
ms.assetid: 8be9e2aa-2dc1-406d-8864-7f556de22809
description: "Indicates whether attendees are not allowed to propose a new date/time for the meeting."
---

# PidLidAppointmentNotAllowPropose Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Indicates whether attendees are not allowed to propose a new date/time for the meeting.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |dispidApptNotAllowPropose  <br/> |
|Property set:  <br/> |PSETID_Appointment  <br/> |
|Long ID (LID):  <br/> |0x0000825A  <br/> |
|Data type:  <br/> |PT_BOOLEAN  <br/> |
|Area:  <br/> |Meetings  <br/> |
   
## Remarks

A value of FALSE, or the absence of this property indicates that the attendees are allowed to propose a new date/time.
  
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

