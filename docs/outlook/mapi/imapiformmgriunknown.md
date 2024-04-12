---
title: "IMAPIFormMgr  IUnknown"
description: "Describes the properties and vtable order of members for IMAPIFormMgrIUnknown, which enables form viewers to obtain information about and activate form servers."
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IMAPIFormMgr
api_type:
- COM
ms.assetid: 8cbd1a42-7de6-43e0-8c77-7711773843d5
---

# IMAPIFormMgr : IUnknown

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Enables form viewers to obtain information about and activate form servers. 
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapiform.h  <br/> |
|Exposed by:  <br/> |Form manager objects  <br/> |
|Implemented by:  <br/> |Form library providers  <br/> |
|Called by:  <br/> |Form viewers  <br/> |
|Interface identifier:  <br/> |IID_IMAPIFormMgr  <br/> |
|Pointer type:  <br/> |LPMAPIFORMMGR  <br/> |
   
## Vtable order

|Member |Description |
|:-----|:-----|
|[LoadForm](imapiformmgr-loadform.md) <br/> |Starts a form to open an existing message. |
|[ResolveMessageClass](imapiformmgr-resolvemessageclass.md) <br/> |Resolves a message class to its form within a form container, and returns a form information object for that form. |
|[ResolveMultipleMessageClasses](imapiformmgr-resolvemultiplemessageclasses.md) <br/> |Resolves a group of message classes to their forms within a form container, and returns an array of form information objects for those forms. |
|[CalcFormPropSet](imapiformmgr-calcformpropset.md) <br/> |Returns an array of the properties that a group of forms uses. |
|[CreateForm](imapiformmgr-createform.md) <br/> |Launches a form to create a new message based on the form's message class. |
|[SelectForm](imapiformmgr-selectform.md) <br/> |Presents a dialog box that enables the user to select a form, and returns a form information object that describes that form. |
|[SelectMultipleForms](imapiformmgr-selectmultipleforms.md) <br/> |Presents a dialog box that enables the user to select multiple forms, and returns an array of form information objects that describe those forms. |
|[SelectFormContainer](imapiformmgr-selectformcontainer.md) <br/> |Presents a dialog box that enables the user to select a form container, and returns an interface for the container object the user selected. |
|[OpenFormContainer](imapiformmgr-openformcontainer.md) <br/> |Opens an [IMAPIFormContainer](imapiformcontaineriunknown.md) interface for a specific form container. |
|[PrepareForm](imapiformmgr-prepareform.md) <br/> |Downloads a form for opening. |
|[IsInConflict](imapiformmgr-isinconflict.md) <br/> |Determines whether a form can handle its own message conflicts. |
|[GetLastError](imapiformmgr-getlasterror.md) <br/> |Returns a [MAPIERROR](mapierror.md) structure that contains information about the previous error occurring to the form manager object. |
   
## See also



[MAPI Interfaces](mapi-interfaces.md)

