---
title: "IMAPIFormInfo  IMAPIProp"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IMAPIFormInfo
api_type:
- COM
ms.assetid: a9fda518-11ba-42aa-85ef-dd2279e0319d
description: "Gives client applications access to properties that are particular to form definition. The provider can describe a form without activating the form."
---

# IMAPIFormInfo : IMAPIProp

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Gives client applications access to properties that are particular to form definition. By keeping form information in a separate object, the form library provider can describe a form to a client without activating the form.
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapiform.h  <br/> |
|Exposed by:  <br/> |Form information objects  <br/> |
|Implemented by:  <br/> |Form library providers  <br/> |
|Called by:  <br/> |Client applications  <br/> |
|Interface identifier:  <br/> |IID_IMAPIFormInfo  <br/> |
|Pointer type:  <br/> |LPMAPIFORMINFO  <br/> |
|Transaction model:  <br/> |Nontransacted  <br/> |
   
## Vtable order

|Member |Description |
|:-----|:-----|
|[CalcFormPropSet](imapiforminfo-calcformpropset.md) <br/> |Returns a pointer to the complete set of properties that a form uses. |
|[CalcVerbSet](imapiforminfo-calcverbset.md) <br/> |Returns a pointer to the complete set of verbs that a form uses. |
|[MakeIconFromBinary](imapiforminfo-makeiconfrombinary.md) <br/> |Builds an icon from an icon property of a form. |
|[SaveForm](imapiforminfo-saveform.md) <br/> |Saves a description of a particular form in a configuration file. |
|[OpenFormContainer](imapiforminfo-openformcontainer.md) <br/> |Returns a pointer to the form container in which a particular form is installed. |
   
## Remarks

Unlike most interfaces defined in the MapiForm.h header file, **IMAPIFormInfo** inherits from the [IMAPIProp](imapipropiunknown.md) interface, because it exports most form information through calls to the [IMAPIProp::GetProps](imapiprop-getprops.md) method. 
  
## See also



[MAPI Interfaces](mapi-interfaces.md)

