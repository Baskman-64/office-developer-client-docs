---
title: "PidTagFreeBusyRangeTimestamp Canonical Property"
description: Outlines the PidTagFreeBusyRangeTimestamp canonical property, which contains the time when the data was published.
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagFreeBusyRangeTimestamp
api_type:
- HeaderDef
ms.assetid: 142d955f-f92d-485a-80c9-9c72e82af0f2
---

# PidTagFreeBusyRangeTimestamp Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains the time when the data was published.
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |PR_FREEBUSY_RANGE_TIMESTAMP  <br/> |
|Identifier:  <br/> |0x6868  <br/> |
|Data type:  <br/> |PT_SYSTIME  <br/> |
|Area:  <br/> |Free/Busy  <br/> |
   
## Remarks

This property is the number of minutes since midnight, January 1, 1601 in Coordinated Universal Time (UTC).
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]](https://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> Provides references to related Exchange Server protocol specifications.
    
[[MS-OXOPFFB]](https://msdn.microsoft.com/library/1a527299-7211-4d27-a74c-b69bd0746320%28Office.15%29.aspx)
  
> Publishes the availability of a user or resource.
    
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

