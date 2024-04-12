---
title: "IFreeBusyData"
manager: lindalu
ms.date: 12/08/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: c9a80ad3-6311-fe07-b6f7-9fd63424753b
---

# IFreeBusyData

For a given user, gets and sets a time range and returns an interface for enumerating free/busy blocks of data within this time range.
  
## Quick info

|Property |Value |
|:-----|:-----|
|Inherits from:  <br/> |[IUnknown](https://msdn.microsoft.com/library/33f1d79a-33fc-4ce5-a372-e08bda378332%28Office.15%29.aspx) <br/> |
|Provided by:  <br/> |Free/busy provider  <br/> |
|Interface identifier:  <br/> |IID_IFreeBusyData  <br/> |
   
## Vtable order

|Member |Description |
|:-----|:-----|
|[Placeholder1](ifreebusydata-placeholder1.md) <br/> | *This member is a placeholder and is not supported.*  <br/> |
|[EnumBlocks](ifreebusydata-enumblocks.md) <br/> |Gets an interface that enumerates free/busy blocks of data for a user within a specified time range. |
|[Placeholder2](ifreebusydata-placeholder2.md) <br/> | *This member is a placeholder and is not supported.*  <br/> |
|[Placeholder3](ifreebusydata-placeholder3.md) <br/> | *This member is a placeholder and is not supported.*  <br/> |
|[Placeholder4](ifreebusydata-placeholder4.md) <br/> | *This member is a placeholder and is not supported.*  <br/> |
|[Placeholder5](ifreebusydata-placeholder5.md) <br/> | *This member is a placeholder and is not supported.*  <br/> |
|[SetFBRange](ifreebusydata-setfbrange.md) <br/> |Sets the range of time for an enumeration of free/busy blocks of data for a user. |
|[Placeholder6](ifreebusydata-placeholder6.md) <br/> | *This member is a placeholder and is not supported.*  <br/> |
|[GetFBPublishRange](ifreebusydata-getfbpublishrange.md) <br/> |Gets a preset time range for an enumeration of free/busy blocks of data for a user. |
   
## Remarks

Most of the members in this interface are placeholders reserved for the internal use of Outlook and are subject to change. Free/busy providers must implement them only as specified, returning only the specified return values.
  
## See also

- [About the Free/Busy API](about-the-free-busy-api.md)
- [Constants (Free/busy API)](constants-free-busy-api.md)

