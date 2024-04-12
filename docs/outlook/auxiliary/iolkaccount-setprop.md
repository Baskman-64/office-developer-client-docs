---
title: "IOlkAccountSetProp"
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 883b1c5d-47dd-a006-b5f1-130691bdd019
description: "Sets the value of the specified account property."
---

# IOlkAccount::SetProp

Sets the value of the specified account property.
  
## Quick info

See [IOlkAccount](iolkaccount.md).
  
```cpp
HRESULT IOlkAccount::SetProp(  
    DWORD dwProp, 
    ACCT_VARIANT *pVar 
);
```

## Parameters

_dwProp_
  
> [in] The property tag of the account property to set.
    
_pVar_
  
> [in] The value of the specified property.
    
## Return values

|**HRESULT**|**Description**|
|:-----|:-----|
|S_OK  <br/> |The method call was successful. |
|E_INVALIDARG  <br/> |An invalid property tag was specified. |
   
## Remarks

Use [IOlkAccount::SaveChanges](iolkaccount-savechanges.md) to save changes to the value of account properties. 
  
## See also

- [Constants (Account management API)](constants-account-management-api.md) 
- [IOlkAccount::GetProp](iolkaccount-getprop.md)

