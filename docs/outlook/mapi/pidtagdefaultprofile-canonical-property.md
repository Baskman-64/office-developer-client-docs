---
title: "PidTagDefaultProfile Canonical Property"
description: Outlines the PidTagDefaultProfile canonical property, which contains TRUE if a messaging user profile is the MAPI default profile.
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagDefaultProfile
api_type:
- HeaderDef
ms.assetid: 47f745a4-5a9c-42af-b076-a72548ef4d31
---

# PidTagDefaultProfile Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains TRUE if a messaging user profile is the MAPI default profile.
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |PR_DEFAULT_PROFILE  <br/> |
|Identifier:  <br/> |0x3D04  <br/> |
|Data type:  <br/> |PT_BOOLEAN  <br/> |
|Area:  <br/> |MAPI profile  <br/> |
   
## Remarks

This property does not appear as a property of any object but only as a column in a profile table. A client application can use the [IProfAdmin::SetDefaultProfile](iprofadmin-setdefaultprofile.md) method to designate the default profile. 
  
## Related resources

### Header files

Mapidefs.h
  
> Provides data type definitions.
    
Mapitags.h
  
> Contains definitions of properties listed as associated properties.
    
## See also



[PidTagDefaultStore Canonical Property](pidtagdefaultstore-canonical-property.md)


[MAPI Properties](mapi-properties.md)
  
[MAPI Canonical Properties](mapi-canonical-properties.md)
  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)
  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)

