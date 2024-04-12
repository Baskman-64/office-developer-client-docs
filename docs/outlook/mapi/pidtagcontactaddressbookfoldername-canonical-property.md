---
title: "PidTagContactAddressBookFolderName Canonical Property"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagContactAddressBookFolderName
api_type:
- HeaderDef
ms.assetid: 6149da2f-6e42-429c-bcdb-d517d21df720
description: "Contains a folder name used for address book entries for Outlook 2013 or Outlook 2016."
---

# PidTagContactAddressBookFolderName Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains a folder name used for address book entries.
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |PR_CONTAB_FOLDER_NAME, PR_CONTAB_FOLDER_NAME_W  <br/> |
|Identifier:  <br/> |0x6613  <br/> |
|Data type:  <br/> |PT_UNICODE, PT_STRING8  <br/> |
|Area:  <br/> |Contact address book  <br/> |
   
## Remarks

The following characters cannot be used in folder names:
  
[ ] / \ &amp; ~ ? \* | \< \> " ; : +
  
## Related resources

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

