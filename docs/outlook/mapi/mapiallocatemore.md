---
title: "MAPIAllocateMore"
description: Describes the MAPIAllocateMore function and provides, syntax, parameters, return value, and additional remarks.
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- MAPIAllocateMore
api_type:
- HeaderDef
ms.assetid: 3e48f76a-bc97-4cbc-9082-c07dd674b73e
---

# MAPIAllocateMore

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Allocates a memory buffer that is linked to another buffer previously allocated with the [MAPIAllocateBuffer](mapiallocatebuffer.md) function. 
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapix.h  <br/> |
|Implemented by:  <br/> |MAPI  <br/> |
|Called by:  <br/> |Client applications and service providers  <br/> |
   
```cpp
SCODE MAPIAllocateMore(
  ULONG cbSize,
  LPVOID lpObject,
  LPVOID FAR * lppBuffer
);
```

## Parameters

 _cbSize_
  
> [in] Size, in bytes, of the new buffer to be allocated. 
    
 _lpObject_
  
> [in] Pointer to an existing MAPI buffer allocated using **MAPIAllocateBuffer**.
    
 _lppBuffer_
  
> [out] Pointer to the returned, newly allocated buffer.
    
## Return value

S_OK 
  
> The call succeeded and has returned a pointer to the requested memory.
    
## Remarks

During **MAPIAllocateMore** call processing, the calling implementation acquires a block of memory from the operating system. The memory buffer is allocated on an even-numbered byte address. On platforms where long integer access is more efficient, the operating system allocates the buffer on an address whose size in bytes is a multiple of four. 
  
The only way to release a buffer allocated with **MAPIAllocateMore** is to pass the buffer pointer specified in the _lpObject_ parameter to the [MAPIFreeBuffer](mapifreebuffer.md) function. The link between the memory buffers allocated with [MAPIAllocateBuffer](mapiallocatebuffer.md) and **MAPIAllocateMore** enables **MAPIFreeBuffer** to release both buffers with a single call. 
  

