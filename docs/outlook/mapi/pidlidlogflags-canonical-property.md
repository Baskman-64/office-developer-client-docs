---
title: "PidLidLogFlags Canonical Property"
description: Outlines the PidLidLogFlags canonical property, which contains metadata about the journal and applies to Outlook 2013 and Outlook 2016.
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidLidLogFlags
api_type:
- COM
ms.assetid: 3174d931-e045-44db-a203-a27c9c00f4fc
---

# PidLidLogFlags Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains metadata about the journal.
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |dispidLogFlags  <br/> |
|Property set:  <br/> |PSETID_Log  <br/> |
|Long ID (LID):  <br/> |0x0000870C  <br/> |
|Data type:  <br/> |PT_LONG  <br/> |
|Area:  <br/> |Journal  <br/> |
   
## Remarks

The bit field that contains metadata about the journal must be either zero or "0x40000000".
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]](https://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> Provides property set definitions and references to related Exchange Server protocol specifications.
    
[[MS-OXOJRNL]](https://msdn.microsoft.com/library/2aa04fd2-0f36-4ce4-9178-c0fc70aa8d43%28Office.15%29.aspx)
  
> Specifies the properties and operations that are permissible for journals.
    
### Header files

Mapidefs.h
  
> Provides data type definitions.
    
## See also



[MAPI Properties](mapi-properties.md)
  
[MAPI Canonical Properties](mapi-canonical-properties.md)
  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)
  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)

