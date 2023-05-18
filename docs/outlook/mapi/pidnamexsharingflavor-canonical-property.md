---
title: "PidNameXSharingFlavor Canonical Property"
description: Outlines the PidNameXSharingFlavor canonical property, which represents the value of the dispidSharingFlavor property.
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidNameXSharingFlavor
api_type:
- COM
ms.assetid: 7757fde1-564b-4f3a-9b9e-f80a143690ea
---

# PidNameXSharingFlavor Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Represents the value of the **dispidSharingFlavor** ([PidLidSharingFlavor](pidlidsharingflavor-canonical-property.md)) property.
  
|Property |Value |
|:-----|:-----|
|Friendly names:  <br/> |None  <br/> |
|Property set:  <br/> |PS_INTERNET_HEADERS  <br/> |
|Property name:  <br/> |X-Sharing-Flavor  <br/> |
|Data type:  <br/> |PT_UNICODE  <br/> |
|Area:  <br/> |Sharing  <br/> |
   
## Remarks

The **dispidSharingFlavor** property must be one of the following values. 
  
|**Value**|**Type of Sharing Message**|
|:-----|:-----|
|0x00020310  <br/> |A sharing invitation for a special folder. |
|0x00000310  <br/> |A sharing invitation for a folder that is not a special folder. |
|0x00020500  <br/> |A sharing request. |
|0x00020710  <br/> |Both a sharing invitation for a special folder and a sharing request for the recipient's equivalent special folder. |
|0x00025100  <br/> |A sharing response that denies a request. |
|0x00023310  <br/> |A sharing response that accepts a request (also a type of sharing invitation). |
   
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

