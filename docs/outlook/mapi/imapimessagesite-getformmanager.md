---
title: "IMAPIMessageSiteGetFormManager"
description: "IMAPIMessageSiteGetFormManager returns a form manager interface, which a form server can use to open another form server."
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IMAPIMessageSite.GetFormManager
api_type:
- COM
ms.assetid: d48bd537-c562-4deb-8a4c-011208991054
---

# IMAPIMessageSite::GetFormManager

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Returns a form manager interface, which a form server can use to open another form server.
  
```cpp
HRESULT GetFormManager(
  LPMAPIFORMMGR FAR * ppFormMgr
);
```

## Parameters

 _ppFormMgr_
  
> [out] A pointer to a pointer to the returned form manager interface.
    
## Return value

S_OK 
  
> The call succeeded and has returned the expected value or values.
    
## Remarks

For a list of interfaces related to form servers, see [MAPI Form Interfaces](mapi-form-interfaces.md).
  
## MFCMAPI reference

For MFCMAPI sample code, see the following table.
  
|**File**|**Function**|**Comment**|
|:-----|:-----|:-----|
|MyMAPIFormViewer.cpp  <br/> |CMyMAPIFormViewer::GetFormManager  <br/> |MFCMAPI uses the **IMAPIMessageSite::GetFormManager** method to call [MAPIOpenFormMgr](mapiopenformmgr.md) and return the results of that call. |
   
## See also



[MAPIOpenFormMgr](mapiopenformmgr.md)
  
[IMAPIMessageSite : IUnknown](imapimessagesiteiunknown.md)


[MFCMAPI as a Code Sample](mfcmapi-as-a-code-sample.md)
  
[MAPI Form Interfaces](mapi-form-interfaces.md)

