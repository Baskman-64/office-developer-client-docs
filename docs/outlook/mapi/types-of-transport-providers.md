---
title: "Types of Transport Providers"
description: Outlines how transport providers support a range of standard features in Outlook 2013 and Outlook 2016.
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.localizationpriority: medium
api_type:
- COM
ms.assetid: 772ecab1-7e91-415b-bae8-af8ffb7b7ed9
 
 
---

# Types of Transport Providers

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
All transport providers support a range of standard features, such as:
  
- Providing proper security for the underlying messaging system.
    
- Sending and receiving messages from the underlying messaging system.
    
- Exposing the address types the transport providers support so the MAPI spooler and client applications can use them appropriately.
    
- Accepting delivery for specific recipients.
    
In addition, MAPI supports two specialized types of providers for specific messaging systems.
  
|**Transport type**|**Added functionality**|
|:-----|:-----|
|Remote Transport  <br/> |Enables interoperability with clients connected remotely. |
|TNEF Transport  <br/> |Allows MAPI properties to be preserved on messaging systems that do not support them. |
   
TNEF transports are used for translating messages between messaging systems that support different sets of MAPI properties. TNEF transports use the MAPI [ITnef : IUnknown](itnefiunknown.md) interface to convert any properties that the destination system cannot represent directly into a binary data stream that can be attached to the message. Later, another TNEF transport can use **ITnef** to decode the data stream and make the original MAPI properties available to client applications. Additionally, TNEF support is required if your transport needs to support custom message classes. For information about implementing TNEF transports, see [Developing a TNEF-Enabled Transport Provider](developing-a-tnef-enabled-transport-provider.md).
  
If your transport provider is not one of these types, you will have to implement it with the basic MAPI functions and networking functions available on your target platform.
  

