---
title: "IXPLogonPoll"
 
 
manager: lindalu
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IXPLogon.Poll
api_type:
- COM
ms.assetid: 1524eb06-7492-42de-b455-e0982bda7ece
---

# IXPLogon::Poll

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Indicates whether the transport provider has received one or more inbound messages.
  
```cpp
HRESULT Poll(
  ULONG FAR * lpulIncoming
);
```

## Parameters

 _lpulIncoming_
  
> [out] A value that indicates the existence of inbound messages. A nonzero value indicates that there are inbound messages.
    
## Return value

S_OK 
  
> The call succeeded and has returned the expected value or values.
    
## Remarks

The MAPI spooler periodically calls the **IXPLogon::Poll** method if the transport provider indicates it must be polled for new messages, which the provider does by passing the LOGON_SP_POLL flag to the call to the [IXPProvider::TransportLogon](ixpprovider-transportlogon.md) method at the beginning of a session. If the transport provider indicates in response to the **Poll** call that there are one or more inbound messages available for it to process, the MAPI spooler calls the [IXPLogon::StartMessage](ixplogon-startmessage.md) method to allow the provider to process the first inbound message. The transport provider indicates inbound messages by setting the value in the _lpulIncoming_ parameter to a nonzero value. 
  
## See also



[IXPLogon::StartMessage](ixplogon-startmessage.md)
  
[IXPProvider::TransportLogon](ixpprovider-transportlogon.md)
  
[IXPLogon : IUnknown](ixplogoniunknown.md)

