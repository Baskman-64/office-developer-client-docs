---
title: "PidTagExtendedRuleMessageCondition Canonical Property"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagExtendedRuleMessageCondition
api_type:
- HeaderDef
ms.assetid: 891851e1-e4a4-4c20-a26c-7223bcca35f7
description: "Contains information about any named properties that are contained inside of extended rule conditions."
---

# PidTagExtendedRuleMessageCondition Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains information about any named properties that are contained inside of extended rule conditions.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |PR_EXTENDED_RULE_MSG_CONDITION  <br/> |
|Identifier:  <br/> |0x0E9A  <br/> |
|Data type:  <br/> |PT_BINARY  <br/> |
|Area:  <br/> |Rules  <br/> |
   
## Remarks

This property must be set on an FAI message. It serves the same purpose as **PR_RULE_CONDITION** ([PidTagRuleCondition](pidtagrulecondition-canonical-property.md)), but contains additional information about the named properties used. All string values contained in any part of this condition property value must be in Unicode format.
  
For information about the format of this binary property, see [[MS-OXORULE]](https://msdn.microsoft.com/library/70ac9436-501e-43e2-9163-20d2b546b886%28Office.15%29.aspx).
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]](https://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> Provides references to related Exchange Server protocol specifications.
    
[[MS-OXORULE]](https://msdn.microsoft.com/library/70ac9436-501e-43e2-9163-20d2b546b886%28Office.15%29.aspx)
  
> Manipulates incoming email messages on a server.
    
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

