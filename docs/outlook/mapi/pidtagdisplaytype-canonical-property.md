---
title: "PidTagDisplayType Canonical Property"
description: Outlines the PidTagDisplayType canonical property, which contains a value used to associate an icon with a particular row of a table. 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagDisplayType
api_type:
- HeaderDef
ms.assetid: ee2bc6ca-3769-4b56-a77d-81418d28f768
---

# PidTagDisplayType Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains a value used to associate an icon with a particular row of a table. 
  
|Property|Value|
|:-----|:-----|
|Associated properties:  <br/> |PR_DISPLAY_TYPE  <br/> |
|Identifier:  <br/> |0x3900  <br/> |
|Data type:  <br/> |PT_LONG  <br/> |
|Area:  <br/> |MAPI address book  <br/> |
   
## Remarks

This property contains a long integer that facilitates special treatment of the table entry based on its type. This special treatment typically consists of displaying an icon, or other display element, associated with the display type. 
  
This property is not used in folder contents tables. Client applications should use a message's **PR_MESSAGE_CLASS** ([PidTagMessageClass](pidtagmessageclass-canonical-property.md)) property and appropriate [IMAPIFormInfo](imapiforminfoimapiprop.md) interface to get the **PR_ICON** ([PidTagIcon](pidtagicon-canonical-property.md)) and **PR_MINI_ICON** ([PidTagMiniIcon](pidtagminiicon-canonical-property.md)) properties for that message. 
  
This property can have exactly one of the following values:
  
DT_AGENT 
  
> An automated agent, such as Quote-Of-The-Day or a weather chart display.
    
DT_DISTLIST 
  
> A distribution list.
    
DT_FOLDER 
  
> Display default folder icon adjacent to folder.
    
DT_FOLDER_LINK 
  
> Display default folder link icon adjacent to folder rather than the default folder icon.
    
DT_FOLDER_SPECIAL 
  
> Display icon for a folder with an application-specific distinction, such as a special type of public folder.
    
DT_FORUM 
  
> A forum, such as a bulletin board service or a public or shared folder.
    
DT_GLOBAL 
  
> A global address book.
    
DT_LOCAL 
  
> A local address book that you share with a small workgroup.
    
DT_MAILUSER 
  
> A typical messaging user.
    
DT_MODIFIABLE 
  
> Modifiable; the container should be denoted as modifiable in the user interface.
    
DT_NOT_SPECIFIC 
  
> Does not match any of the other settings.
    
DT_ORGANIZATION 
  
> A special alias defined for a large group, such as helpdesk, accounting, or blood-drive coordinator.
    
DT_PRIVATE_DISTLIST 
  
> A private, personally administered distribution list.
    
DT_REMOTE_MAILUSER 
  
> A recipient known to be from a foreign or remote messaging system.
    
DT_WAN 
  
> A wide area network address book.
    
Address book contents tables use the DT_AGENT, DT_DISTLIST, DT_FORUM, DT_MAILUSER, DT_ORGANIZATION, DT_PRIVATE_DISTLIST, and DT_REMOTE_MAILUSER values. Address book hierarchy tables and one-off tables use the DT_GLOBAL, DT_LOCAL, DT_MODIFIABLE, DT_NOT_SPECIFIC, and DT_WAN values. Folder hierarchy tables use the DT_FOLDER, DT_FOLDER_LINK, and DT_FOLDER_SPECIAL values. 
  
If this property is not set, the client should assume the default type appropriate for the table, typically DT_FOLDER, DT_LOCAL, or DT_MAILUSER. 
  
 **Note** All values not documented are reserved for MAPI. Client applications must not define any new values and must be prepared to deal with an undocumented value. 
  
## Related resources

### Protocol specifications

[[MS-OXPROPS]](https://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> Provides references to related Exchange Server protocol specifications.
    
[[MS-OXCMSG]](https://msdn.microsoft.com/library/7fd7ec40-deec-4c06-9493-1bc06b349682%28Office.15%29.aspx)
  
> Handles message and attachment objects.
    
[[MS-OXOABK]](https://msdn.microsoft.com/library/f4cf9b4c-9232-4506-9e71-2270de217614%28Office.15%29.aspx)
  
> Specifies the properties and operations that are permissible for address book templates.
    
[[MS-OXLDAP]](https://msdn.microsoft.com/library/727c090a-f05c-4eed-94aa-565724cfc550%28Office.15%29.aspx)
  
> Enables directory access.
    
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

