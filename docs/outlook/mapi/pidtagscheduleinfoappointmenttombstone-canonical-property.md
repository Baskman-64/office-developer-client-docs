---
title: "PidTagScheduleInfoAppointmentTombstone Canonical Property"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.PidTagScheduleInfoAppointmentTombstone
api_type:
- COM
ms.assetid: 6b82e2ee-992f-4cbe-bdcb-e7465e556640
description: "Contains a list of data blocks that represent meetings which have been declined for Outlook 2013 or Outlook 2016."
---

# PidTagScheduleInfoAppointmentTombstone Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains a list of data blocks that represent meetings that have been declined.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |PR_SCHDINFO_APPT_TOMBSTONE  <br/> |
|Identifier:  <br/> |0x686A  <br/> |
|Data type:  <br/> |PT_BINARY  <br/> |
|Area:  <br/> |Free/Busy  <br/> |
   
## Remarks

The data blocks begin with a header of 32 bit values defined as:
  
|**Value**|**Description**|
|:-----|:-----|
|Identifier  <br/> |This field must be the value 0xBEDEAFCD. |
|HeaderSize  <br/> |This field must have the value 0x00000014. |
|Version  <br/> |This field must have the value 3. |
|RecordsCount  <br/> |The count of records that follow. |
|RecordsSize  <br/> |This field must have the value 0x00000014. |
   
The header is followed by **RecordsCount** entries of 32 bit values defined as: 
  
|**Value**|**Description**|
|:-----|:-----|
|StartTime  <br/> |The meeting object's start time in minutes since midnight, January 1, 1601, UTC. |
|EndTime  <br/> |The meeting object's end time in minutes since midnight, January 1, 1601, UTC. |
|GlobalObjectIdSize  <br/> |The size, in bytes, of the GlobalObjectId field. |
|GlobalObjectId  <br/> |The value of the **LID_GLOBAL_OBJID** ([PidLidGlobalObjectId](pidlidglobalobjectid-canonical-property.md)) property of the meeting this record represents. |
|UserName  <br/> |The first two bytes are the length of the PT_STRING8 string that follows. |
   
## Related resources

### Protocol specifications

[[MS-OXPROPS]](https://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> Provides references to related Exchange Server protocol specifications.
    
[[MS-OXOCAL]](https://msdn.microsoft.com/library/09861fde-c8e4-4028-9346-e7c214cfdba1%28Office.15%29.aspx)
  
> Specifies the properties and operations for appointment, meeting request, and response messages.
    
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

