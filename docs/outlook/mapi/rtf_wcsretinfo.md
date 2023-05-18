---
title: "RTF_WCSRETINFO"
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
ms.assetid: 62561d8d-33cb-e482-7fa0-132afe2b464a
description: "This structure provides information about a stream in native format returned from decompressing the body of a message that is encapsulated in compressed RTF."
---

# RTF_WCSRETINFO

**Applies to**: Outlook 2013 | Outlook 2016 
  
This structure provides information about a stream in native format returned from decompressing the body of a message that is encapsulated in compressed Rich Text Format (RTF).
  
## Quick info

```cpp
typedef struct { 
    ULONG size;    
    ULONG ulStreamFlags; 
} RTF_WCSRETINFO;
```

## Members

_size_
  
> The size of the **RTF_WCSRETINFO** structure in number of bytes. 
    
_ulStreamFlags_
  
> This is a value that indicates the format of the native body. This value is only valid if the **MAPI_NATIVE_BODY** flag is passed in the _ulFlags_ parameter of the [RTF_WCSINFO](rtf_wcsinfo.md) structure that is passed to the [WrapCompressedRTFStreamEx](wrapcompressedrtfstreamex.md) function. This can be one of the following values: 
    
|Value |Description |
|:-----|:-----|
|MAPI_NATIVE_BODY_TYPE_RTF  <br/> |This value is only used if  _ulFlags_ includes the **MAPI_NATIVE_BODY** flag, and the body is RTF. |
|MAPI_NATIVE_BODY_TYPE_PLAIN_TEXT  <br/> |This value is only used if  _ulFlags_ includes the **MAPI_NATIVE_BODY** flag, and the body is plain text format. |
|MAPI_NATIVE_BODY_TYPE_HTML  <br/> |This value is only used if  _ulFlags_ includes the **MAPI_NATIVE_BODY** flag, and the body is Hypertext Markup Language (HTML) format. |
   
## See also

- [WrapCompressedRTFStreamEx](wrapcompressedrtfstreamex.md)

