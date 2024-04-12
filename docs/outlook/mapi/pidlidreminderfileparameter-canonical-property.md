---
title: "PidLidReminderFileParameter Canonical Property"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidLidReminderFileParameter
api_type:
- COM
ms.assetid: 1009f0ea-6f35-484d-b04d-5b6e844c14dd
description: "Specifies the filename of the sound that a client should play when the reminder for that object becomes overdue."
---

# PidLidReminderFileParameter Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Specifies the filename of the sound that a client should play when the reminder for that object becomes overdue.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |dispidReminderFileParam  <br/> |
|Property set:  <br/> |PSETID_Common  <br/> |
|Long ID (LID):  <br/> |0x0000851F  <br/> |
|Data type:  <br/> |PT_UNICODE  <br/> |
|Area:  <br/> |Reminder  <br/> |
   
## Remarks

If this property is not present, the client may use a default value.
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]](https://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> Provides property set definitions and references to related Exchange Server protocol specifications.
    
[[MS-OXORMDR]](https://msdn.microsoft.com/library/5454ebcc-e5d1-4da8-a598-d393b101caab%28Office.15%29.aspx)
  
> Specifies the properties and the interaction model for email and other object reminders.
    
### Header files

Mapidefs.h
  
> Provides data type definitions.
    
## See also



[MAPI Properties](mapi-properties.md)
  
[MAPI Canonical Properties](mapi-canonical-properties.md)
  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)
  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)

