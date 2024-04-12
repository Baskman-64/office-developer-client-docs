---
title: "MAPI Service Provider Objects"
description: "Describes all the MAPI service provider objects, which are strictly for bookkeeping; they are used by MAPI to control the startup and shutdown processes."
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.localizationpriority: medium
api_type:
- COM
ms.assetid: f8ade454-2450-49e6-a76f-93801055a7e5
 
 
---

# MAPI Service Provider Objects

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Service providers implement many objects. Some are used primarily by MAPI and some are used by client applications. A few objects are implemented by all types of service providers; the rest are specific to a single provider type. The following table describes all of the service provider objects.
  
|**Service provider object**|**Description**|
|:-----|:-----|
|Address book container  <br/> |Contains recipient information for one address book provider in the active profile; address book providers can have one or more address book containers. |
|Attachment  <br/> |Contains additional data, such as a file or OLE object, to be associated with a message. |
|Control  <br/> |Enables or disables a button and initiates processing when the button is clicked. |
|Distribution list  <br/> |Describes a grouping of individual message recipients. |
|Folder  <br/> |Contains messages and other message containers. |
|Logon  <br/> |Handles service provider event notification and client requests. |
|Messaging user  <br/> |Describes an individual recipient of a message. |
|Message  <br/> |Contains information that can be sent to one or more recipients. |
|Message store  <br/> |Acts as a hierarchically organized database of messages. |
|Provider  <br/> |Handles service provider startup and shutdown. |
|Spooler hook  <br/> |Performs special processing on inbound and outbound messages. |
|Status  <br/> |Provides access to the service provider's state. |
|Table  <br/> |Provides access to a summary view of object data in row and column format, similar to a database table. |
   
All service providers implement a provider object and a logon object. Provider objects are strictly for bookkeeping; they are used by MAPI to control the startup and shutdown processes. Logon objects service some client requests indirectly. For example, the message store provider's logon object handles notification registration and requests to open message store objects. 
  
Provider and logon objects implement a different interface depending on the type of service provider that supplies the implementation. A message store provider implements the [IMSProvider : IUnknown](imsprovideriunknown.md) and [IMSLogon : IUnknown](imslogoniunknown.md) interfaces in its provider and logon objects, an address book provider implements the [IABProvider : IUnknown](iabprovideriunknown.md) and [IABLogon : IUnknown](iablogoniunknown.md) interfaces, and a transport provider implements the [IXPProvider : IUnknown](ixpprovideriunknown.md) and [IXPLogon : IUnknown](ixplogoniunknown.md) interfaces. 
  
Message hook providers implement spooler hook objects, or objects that filter inbound and outbound messages.
  
Service providers typically use only a few objects. Most frequently, they use a support object that MAPI provides to help implement client requests. The support object is customized for the type of provider that is using it. For all service providers, the support object includes methods for handling event notification, displaying configuration properties, opening objects, and error handling. The rest of the methods are specific to its use; there are customized versions for address book, message store, and transport providers, and for configuration support. For example, the address book support object displays details and custom recipient dialog boxes. The message store support object supports copy and move operations for folders and messages. The transport provider support object includes methods for facilitating interaction with the MAPI spooler. 
  
Some service providers use table data and property data objects — utility objects that MAPI implements. Table data objects enable service providers to manage the underlying data of a table. Property data objects enable service providers to set object and property access. 
  
Transport providers that support the Transport Neutral Encapsulation Format (TNEF) for transferring properties use a TNEF object that MAPI implements to support the [ITnef : IUnknown](itnefiunknown.md) interface. For more information, see [Developing a TNEF-Enabled Transport Provider](developing-a-tnef-enabled-transport-provider.md). 
  
## See also



[ITnef : IUnknown](itnefiunknown.md)
  
[IMSProvider : IUnknown](imsprovideriunknown.md)
  
[IMSLogon : IUnknown](imslogoniunknown.md)
  
[IABProvider : IUnknown](iabprovideriunknown.md)
  
[IABLogon : IUnknown](iablogoniunknown.md)
  
[IXPProvider : IUnknown](ixpprovideriunknown.md)
  
[IXPLogon : IUnknown](ixplogoniunknown.md)


[Developing a TNEF-Enabled Transport Provider](developing-a-tnef-enabled-transport-provider.md)

