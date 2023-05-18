---
title: "IMsgServiceAdmin2  IMsgServiceAdmin"
description: "Describes the properties and vtable order of members for IMsgServiceAdmin2 IMsgServiceAdmin, which makes changes to a message service in a profile."
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IMsgServiceAdmin2
api_type:
- COM
ms.assetid: 14654259-e884-46bf-84ff-9e3c1a8cd60d
---

# IMsgServiceAdmin2 : IMsgServiceAdmin

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Makes changes to a message service in a profile.
  
|Property|Value|
|:-----|:-----|
|Header file:  <br/> |Mapiaux.h  <br/> |
|Exposed by:  <br/> |Message service administration objects  <br/> |
|Implemented by:  <br/> |MAPI  <br/> |
|Called by:  <br/> |Client applications  <br/> |
|Interface identifier:  <br/> |IID_IMsgServiceAdmin2  <br/> |
|Pointer type:  <br/> |LPSERVICEADMIN2  <br/> |
   
## Vtable order

|Member|Description|
|:-----|:-----|
|[CreateMsgServiceEx](imsgserviceadmin2-createmsgserviceex.md) <br/> |Adds a message service to the current profile and returns that newly added service UID. |
   
## Remarks

The **IMsgServiceAdmin2** interface is exposed by the same objects that expose the [IMsgServiceAdmin](imsgserviceadminiunknown.md) interface, and has been available using Outlook's implementation of the MAPI subsystem since Microsoft Outlook 2003. 
  
## See also



[MAPI Interfaces](mapi-interfaces.md)

