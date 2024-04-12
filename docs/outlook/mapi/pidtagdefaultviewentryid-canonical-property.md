---
title: "PidTagDefaultViewEntryId Canonical Property"
description: Outlines the PidTagDefaultViewEntryId canonical property, which contains the entry identifier of a folder's default view.
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagDefaultViewEntryId
api_type:
- HeaderDef
ms.assetid: 1b4e82ed-c207-4828-8a5b-0ef312962355
---

# PidTagDefaultViewEntryId Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains the entry identifier of a folder's default view.
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |PR_DEFAULT_VIEW_ENTRYID  <br/> |
|Identifier:  <br/> |0x3616  <br/> |
|Data type:  <br/> |PT_BINARY  <br/> |
|Area:  <br/> |MAPI container  <br/> |
   
## Remarks

This property is the entry identifier of the folder view that should be set as the initial view. The property need not be set if the "Normal" view is to be used as the initial view.
  
A client application can obtain this property at the time it opens the folder and realize significant performance gains. This property can be used as a shortcut to obtain the default view, instead of opening the associated contents table and submitting a restriction.
  
A service provider implementation of the [IMAPIFolder::CopyFolder](imapifolder-copyfolder.md) method can copy this property when it copies folders. 
  
## Related resources

### Protocol specifications

[[MS-OXCFOLD]](https://msdn.microsoft.com/library/c0f31b95-c07f-486c-98d9-535ed9705fbf%28Office.15%29.aspx)
  
> Handles folder operations.
    
### Header files

Mapidefs.h
  
> Provides data type definitions.
    
Mapitags.h
  
> Contains definitions of properties listed as associated properties.
    
## See also



[MAPI Properties](mapi-properties.md)
  
[MAPI Canonical Properties](mapi-canonical-properties.md)
  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)
  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)

