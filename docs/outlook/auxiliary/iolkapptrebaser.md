---
title: "IOlkApptRebaser"
manager: lindalu
ms.date: 12/07/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: d67bd395-d324-217d-8ddc-1d48dd724383
description: "Supports rebasing appointments in a calendar folder."
---

# IOlkApptRebaser

Supports rebasing appointments in a calendar folder.
  
## Quick info

|Property |Value |
|:-----|:-----|
|Inherits from:  <br/> |**IUnknown** <br/> |
|Header file:  <br/> |tzmovelib.h  <br/> |
|Implemented by:  <br/> |tzmovelib.dll  <br/> |
|Called by:  <br/> |MAPI client applications  <br/> |
|Exposed on:  <br/> |Outlook rebasing object  <br/> |
   
## Vtable order

||Value |
|:-----|:-----|
|**[BeginEnumerateAppointments](iolkapptrebaser-beginenumerateappointments.md)** <br/> |Begins a task for appointment enumeration in a calendar folder to find the appointments that need rebasing. |
|**[EndEnumerateAppointments](iolkapptrebaser-endenumerateappointments.md)** <br/> |Waits for appointment enumeration in a calendar folder to complete and returns a list of appointments that need rebasing. |
|**[BeginRebaseAppointments](iolkapptrebaser-beginrebaseappointments.md)** <br/> |Begins a task for appointment rebasing given a list of appointments, usually obtained from **EndEnumerateAppointments**. |
|**[EndRebaseAppointments](iolkapptrebaser-endrebaseappointments.md)** <br/> |Waits for appointment rebasing to complete and retrieves the results. |
   
## See also

- [About rebasing calendars programmatically for Daylight Saving Time](about-rebasing-calendars-programmatically-for-daylight-saving-time.md)

