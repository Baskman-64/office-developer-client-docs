---
title: "PidTagScheduleInfoMonthsMerged Canonical Property"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.PidTagScheduleInfoMonthsMerged
api_type:
- COM
ms.assetid: b13b5d7b-413e-4405-8a35-0422477a9e86
description: "Contains a list of the months for which free data of type busy or an out of office (OOF) message is present in the free message."
---

# PidTagScheduleInfoMonthsMerged Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains a list of the months for which free/busy data of type busy or an out of office (OOF) message is present in the free/busy message. 
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |PR_SCHDINFO_MONTHS_MERGED  <br/> |
|Identifier:  <br/> |0x684F  <br/> |
|Data type:  <br/> |PT_MV_LONG  <br/> |
|Area:  <br/> |Free/Busy  <br/> |
   
## Remarks

Events of free/busy type tentative are not included in this property. The syntax/format and constraints of this property are the same as those of **PR_SCHDINFO_MONTHS_TENTATIVE** ([PidTagScheduleInfoMonthsTentative](pidtagscheduleinfomonthstentative-canonical-property.md)) but refer to appointments that are marked OOF or Busy on the associated calendar object. 
  
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

