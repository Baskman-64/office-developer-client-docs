---
title: "PidLidHtml Canonical Property"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidLidHtml
api_type:
- COM
ms.assetid: 5598cbaf-cb9a-4d3a-b123-9108a7aa7c1c
description: "Specifies the contact's business Web page URL. The value of this property, if present, should be the same as the value of the PR_BUSINESS_HOME_PAGE property."
---

# PidLidHtml Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Specifies the contact's business Web page URL.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |dispidHTML  <br/> |
|Property set:  <br/> |PSETID_Address  <br/> |
|Long ID (LID):  <br/> |0x0000802B  <br/> |
|Data type:  <br/> |PT_UNICODE  <br/> |
|Area:  <br/> |Contact  <br/> |
   
## Remarks

The value of this property, if present, should be the same as the value of the **PR_BUSINESS_HOME_PAGE** ([PidTagBusinessHomePage](pidtagbusinesshomepage-canonical-property.md)) property.
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]](https://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> Provides property set definitions and references to related Exchange Server protocol specifications.
    
[[MS-OXOCNTC]](https://msdn.microsoft.com/library/9b636532-9150-4836-9635-9c9b756c9ccf%28Office.15%29.aspx)
  
> Specifies the properties and operations that are permissible for contacts and personal distribution lists.
    
### Header files

Mapidefs.h
  
> Provides data type definitions.
    
## See also



[MAPI Properties](mapi-properties.md)
  
[MAPI Canonical Properties](mapi-canonical-properties.md)
  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)
  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)

