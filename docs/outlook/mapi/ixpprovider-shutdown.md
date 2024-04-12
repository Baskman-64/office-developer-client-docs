---
title: "IXPProviderShutdown"
 
 
manager: lindalu
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IXPProvider.Shutdown
api_type:
- COM
ms.assetid: e2d8a025-c2a3-4edb-b6e4-022e07e854dd
---

# IXPProvider::Shutdown

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Closes down a transport provider in an orderly fashion.
  
```cpp
HRESULT Shutdown (
  ULONG FAR * lpulFlags
);
```

## Parameters

 _lpulFlags_
  
> [in] Reserved; must be zero.
    
## Return value

S_OK 
  
> The call succeeded in shutting down the transport provider.
    
## Remarks

The MAPI spooler calls the **IXPProvider::Shutdown** method just prior to releasing a transport provider object. Before calling **Shutdown**, MAPI releases all logon objects for a provider.
  
## See also



[XPProviderInit](xpproviderinit.md)
  
[IXPProvider : IUnknown](ixpprovideriunknown.md)

