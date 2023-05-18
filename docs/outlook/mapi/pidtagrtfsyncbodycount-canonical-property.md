---
title: "PidTagRtfSyncBodyCount Canonical Property"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.PidTagRtfSyncBodyCount
api_type:
- COM
ms.assetid: b7267be4-8d5c-4dc7-86b2-651e03e84f9b
description: "Contains a count of the significant characters of the message text. These properties aren't intended to be used directly by client applications."
---

# PidTagRtfSyncBodyCount Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains a count of the significant characters of the message text.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |PR_RTF_SYNC_BODY_COUNT  <br/> |
|Identifier:  <br/> |0x1007  <br/> |
|Data type:  <br/> |PT_LONG  <br/> |
|Area:  <br/> |MAPI message  <br/> |
   
## Remarks

The [RTFSync](rtfsync.md) function computes the count of characters in the text using only those that it considers to be significant to the message. For example, some white space and other ignorable characters are omitted from the count. 
  
This property is a Rich Text Format (RTF) auxiliary property. These properties are used by the **RTFSync** function and are not intended to be used directly by client applications. 
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]](https://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> Provides references to related Exchange Server protocol specifications.
    
[[MS-OXTNEF]](https://msdn.microsoft.com/library/1f0544d7-30b7-4194-b58f-adc82f3763bb%28Office.15%29.aspx)
  
> Encodes and decodes message and attachment objects to an efficient stream representation.
    
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

