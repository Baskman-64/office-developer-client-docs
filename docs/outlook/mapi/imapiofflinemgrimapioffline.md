---
title: "IMAPIOfflineMgr  IMAPIOffline"
description: "IMAPIOfflineMgrIMAPIOffline supports registering for notification callbacks about connection state changes of a user account."
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IMAPIOfflineMgr
api_type:
- COM
ms.assetid: 3e430308-190c-c9bb-fffc-c26ffecb73a5
---

# IMAPIOfflineMgr : IMAPIOffline

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Supports registering for notification callbacks about connection state changes of a user account.
  
|Property|Value|
|:-----|:-----|
|Exported by:  <br/> |msmapi32.dll  <br/> |
|Implemented by:  <br/> |Outlook  <br/> |
|Called by:  <br/> |Client  <br/> |
|Interface identifier:  <br/> |IID_IMAPIOfflineMgr  <br/> |
   
## Vtable order

|Member|Description|
|:-----|:-----|
|[Advise](imapiofflinemgr-advise.md) <br/> |Registers for notification callbacks about connection changes. |
|[Unadvise](imapiofflinemgr-unadvise.md) <br/> |Removes a given registration for notification callbacks. |
| *Placeholder member*  <br/> | *This member is a placeholder and is not supported.*  <br/> |
| *Placeholder member*  <br/> | *This member is a placeholder and is not supported.*  <br/> |
| *Placeholder member*  <br/> | *This member is a placeholder and is not supported.*  <br/> |
| *Placeholder member*  <br/> | *This member is a placeholder and is not supported.*  <br/> |
| *Placeholder member*  <br/> | *This member is a placeholder and is not supported.*  <br/> |
| *Placeholder member*  <br/> | *This member is a placeholder and is not supported.*  <br/> |
| *Placeholder member*  <br/> | *This member is a placeholder and is not supported.*  <br/> |
   
## Remarks

Upon opening an offline object for a user account profile using **[HrOpenOfflineObj](hropenofflineobj.md)**, a client obtains an offline object that supports **IMAPIOfflineMgr**. 
  
Because this interface inherits from **[IUnknown](https://msdn.microsoft.com/library/ms680509%28v=VS.85%29.aspx)**, the client can query this interface (by using **[IUnknown::QueryInterface](https://msdn.microsoft.com/library/ms682521%28v=VS.85%29.aspx)** ) to obtain an object that supports **[IMAPIOffline](imapiofflineiunknown.md)**. The client can then find out about the callback capabilities of the offline object (by calling **[IMAPIOffline::GetCapabilities](imapioffline-getcapabilities.md)** ), and choose to set up callbacks (by using **IMAPIOfflineMgr::Advise** ). 
  
Most of the members in this interface are placeholders reserved for the internal use of Outlook and are subject to change. Callers of this interface must use non-placeholder members only as documented.
  
## See also



[IMAPIOffline : IUnknown](imapiofflineiunknown.md)


[About the Offline State API](about-the-offline-state-api.md)
  
[MAPI Constants](mapi-constants.md)
  
[HrOpenOfflineObj](hropenofflineobj.md)
  
[MAPI Interfaces](mapi-interfaces.md)

