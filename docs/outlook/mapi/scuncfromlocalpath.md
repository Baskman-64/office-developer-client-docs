---
title: "ScUNCFromLocalPath"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.ScUNCFromLocalPath
api_type:
- COM
ms.assetid: cc4abf1a-c08c-4462-9d7c-6af506dc07c9
description: "Locates a universal naming convention (UNC) path counterpart to the given local path for Outlook 2013 or Outlook 2016."
---

# ScUNCFromLocalPath

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Locates a universal naming convention (UNC) path counterpart to the given local path.
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapidefs.h  <br/> |
|Implemented by:  <br/> |MAPI  <br/> |
|Called by:  <br/> |Client applications and service providers  <br/> |
   
```cpp
SCODE ScUNCFromLocalPath(
  LPSTR szLocal,
  LPSTR szUNC,
  UINT cchUNC
);
```

## Parameters

 _szLocal_
  
> [in] A path in the format [ _drive:_]\[ _path_] of a file or directory.
    
 _szUNC_
  
> [out] A path in the format \\[ _server_]\[ _share_]\[ _path_] of the same file or directory as for the  _szLocal_ parameter. 
    
 _cchUNC_
  
> [in] Size of the buffer for the output string.
    
## Return value

S_OK
  
> The UNC path counterpart was successfully located.
    
MAPI_E_INVALID_PARAMETER
  
> One or more parameters are invalid.
    
MAPI_E_TOO_BIG
  
>  _szUNC_ was not large enough to hold the result. 
    
S_FALSE
  
> The local path was already a UNC string.
    
## See also



[ScLocalPathFromUNC](sclocalpathfromunc.md)

