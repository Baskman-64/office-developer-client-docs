---
title: "IMAPIContainer  IMAPIProp"
description: "IMAPIContainerIMAPIProp manages high-level operations on container objects such as address books, distribution lists, and folders."
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IMAPIContainer
api_type:
- COM
ms.assetid: d83fdd83-3e86-43c8-a73f-8e9e01b53371
---

# IMAPIContainer : IMAPIProp

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Manages high-level operations on container objects such as address books, distribution lists, and folders. The [IMAPIFolder : IMAPIContainer](imapifolderimapicontainer.md), [IABContainer : IMAPIContainer](iabcontainerimapicontainer.md), and [IDistList : IMAPIContainer](idistlistimapicontainer.md) interfaces are derived from **IMAPIContainer**.
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapidefs.h  <br/> |
|Exposed by:  <br/> |Folder, address book container, and distribution list objects  <br/> |
|Implemented by:  <br/> |Message store, address book, and remote transport providers  <br/> |
|Called by:  <br/> |Client applications  <br/> |
|Interface identifier:  <br/> |IID_IMAPIContainer  <br/> |
|Pointer type:  <br/> |LPMAPICONTAINER  <br/> |
|Transaction model:  <br/> |Abstract class, never implemented  <br/> |
   
## Vtable order

|Member |Description |
|:-----|:-----|
|[GetContentsTable](imapicontainer-getcontentstable.md) <br/> |Returns a pointer to the container's contents table. |
|[GetHierarchyTable](imapicontainer-gethierarchytable.md) <br/> |Returns a pointer to the container's hierarchy table. |
|[OpenEntry](imapicontainer-openentry.md) <br/> |Opens an object in the container, returning an interface pointer for further access. |
|[SetSearchCriteria](imapicontainer-setsearchcriteria.md) <br/> |Establishes search criteria for the container. |
|[GetSearchCriteria](imapicontainer-getsearchcriteria.md) <br/> |Obtains the search criteria for the container. |
   
|**Required properties**|**Access**|
|:-----|:-----|
|**PR_CONTAINER_HIERARCHY** ([PidTagContainerHierarchy](pidtagcontainerhierarchy-canonical-property.md))  <br/> |Read-only  <br/> |
|**PR_CONTAINER_CONTENTS** ([PidTagContainerContents](pidtagcontainercontents-canonical-property.md))  <br/> |Read-only  <br/> |
|**PR_CONTAINER_FLAGS** ([PidTagContainerFlags](pidtagcontainerflags-canonical-property.md))  <br/> |Read/write  <br/> |
   
## See also



[MAPI Interfaces](mapi-interfaces.md)

