---
title: "PidLidSharingInitiatorEntryId Canonical Property"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidLidSharingInitiatorEntryId
api_type:
- COM
ms.assetid: 47f00706-83df-49cb-bda7-ef572d76a020
description: "Designates as a property of a sharing message. This property must be set to the value of the PR_ENTRYID property for the Address Book of the current user."
---

# PidLidSharingInitiatorEntryId Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Designates as a property of a sharing message.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |dispidSharingInitiatorEid  <br/> |
|Property set:  <br/> |PSETID_Sharing  <br/> |
|Long ID (LID):  <br/> |0x00008A09  <br/> |
|Data type:  <br/> |PT_BINARY  <br/> |
|Area:  <br/> |Sharing  <br/> |
   
## Remarks

This property must be set to the value of the **PR_ENTRYID** ([PidTagEntryId](pidtagentryid-canonical-property.md)) property for the Address Book of the currently logged-on user (see [[MS-OXOABK]](https://msdn.microsoft.com/library/f4cf9b4c-9232-4506-9e71-2270de217614%28Office.15%29.aspx)). 
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]](https://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> Provides property set definitions and references to related Exchange Server protocol specifications.
    
[[MS-OXSHARE]](https://msdn.microsoft.com/library/e4e5bd27-d5e0-43f9-a6ea-550876724f3d%28Office.15%29.aspx)
  
> Shares mailbox folders between clients.
    
### Header files

Mapidefs.h
  
> Provides data type definitions.
    
## See also



[MAPI Properties](mapi-properties.md)
  
[MAPI Canonical Properties](mapi-canonical-properties.md)
  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)
  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)

