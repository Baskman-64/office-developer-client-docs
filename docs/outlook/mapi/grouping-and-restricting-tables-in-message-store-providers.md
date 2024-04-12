---
title: "Grouping and Restricting Tables in Message Store Providers"
description: This article describes grouping and restricting tables in message store providers.
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.localizationpriority: medium
api_type:
- COM
ms.assetid: 01df4be4-98a1-4159-a06d-9ccf4337198f
 
 
---

# Grouping and Restricting Tables in Message Store Providers

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Client applications frequently allow users some control over how the contents of a folder are displayed. Typically, a user can choose to have messages grouped according to the value of one or more message properties, or can choose to exclude messages that match certain criteria. This is done by using the [IMAPITable : IUnknown](imapitableiunknown.md) interface. Client applications can restrict the rows returned from the table to whatever criteria the user specifies. Therefore, a message store provider needs to implement the following **IMAPITable** methods. 
  
|****IMAPITable** method**|**Description**|
|:-----|:-----|
|[IMAPITable::FindRow](imapitable-findrow.md) <br/> |Returns table rows that match the specified criteria. |
|[IMAPITable::QueryColumns](imapitable-querycolumns.md) <br/> |Returns the set of columns in a table or the set of currently used columns. |
|[IMAPITable::QueryRows](imapitable-queryrows.md) <br/> |Returns one or more rows from a table, starting from a given position. |
|[IMAPITable::Restrict](imapitable-restrict.md) <br/> |Applies a restriction to a table so that subsequent calls to **FindRow** return only rows that match the restriction. |
|[IMAPITable::SetColumns](imapitable-setcolumns.md) <br/> |Specifies which columns should be returned when rows are retrieved from the table. |
   
Restrictions can be complex to implement; for more information, see [About Restrictions](about-restrictions.md). For more information about implementing tables, see [MAPI Tables](mapi-tables.md).
  
## See also



[Message Store Features](message-store-features.md)

