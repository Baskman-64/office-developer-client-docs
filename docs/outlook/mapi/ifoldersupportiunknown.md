---
title: "IFolderSupport  IUnknown"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IFolderSupport
api_type:
- COM
ms.assetid: a4b03a66-cf6d-cd20-f1df-b247d3ee87aa
description: "Provides information about a folder's support for sharing. Generally, Outlook requires a MAPI store provider to implement this interface to share a folder."
---

# IFolderSupport : IUnknown

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Provides information about a folder's support for sharing.
  
|Property |Value |
|:-----|:-----|
|Provided by:  <br/> |Message store provider  <br/> |
|Interface identifier:  <br/> |IID_IFolderSupport  <br/> |
   
## Vtable order

|Property |Value |
|:-----|:-----|
|**[GetSupportMask](ifoldersupport-getsupportmask.md)** <br/> |Gets information about a folder's support for sharing. |
   
## Remarks

Generally, Microsoft Office Outlook requires a MAPI store provider to implement this interface if the provider wants to share a folder. The exception is the Exchange Server store provider, which can share folders without implementing this interface.
  
A client can query an **[IMAPIFolder](imapifolderimapicontainer.md)** for **IFolderSupport**. If that succeeds, call **IFolderSupport::GetSupportMask** and check for the **FS_SUPPORTS_SHARING** bit to be set. 
  

