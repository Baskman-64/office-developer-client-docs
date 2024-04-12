---
title: "PidTagExpiryNumber Canonical Property"
description: Outlines the PidTagExpiryNumber canonical property, which defines the expiry send time in conjunction with the PR_EXPIRY_UNITS property.
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagExpiryNumber
api_type:
- HeaderDef
ms.assetid: 644e8d3d-1792-4417-95a1-e978d0e6cd8e
---

# PidTagExpiryNumber Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Defines the expiry send time in conjunction with the **PR_EXPIRY_UNITS** ([PidTagExpiryUnits](pidtagexpiryunits-canonical-property.md)) property.
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |PR_EXPIRY_NUMBER  <br/> |
|Identifier:  <br/> |0x3FED  <br/> |
|Data type:  <br/> |PT_LONG  <br/> |
|Area:  <br/> |MAPI status  <br/> |
   
## Remarks

This property's value must be set between 0 and 999 inclusive, if it is present.
  
## Related resources

### Protocol specifications

[[MS-OXOMSG]](https://msdn.microsoft.com/library/daa9120f-f325-4afb-a738-28f91049ab3c%28Office.15%29.aspx)
  
> Specifies the properties and operations that are permissible for email message objects.
    
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

