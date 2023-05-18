---
title: "IMsgStore  IMAPIProp"
description: "Describes the properties and vtable order of members for IMsgStore IMAPIProp, which provides access to message store information and to messages and folders."
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
api_name:
- IMsgStore
api_type:
- COM
ms.assetid: 20090114-b183-4767-8971-a304a9aa47e6
---

# IMsgStore : IMAPIProp

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Provides access to message store information and to messages and folders.
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapidefs.h  <br/> |
|Exposed by:  <br/> |Message store object  <br/> |
|Implemented by:  <br/> |Message store providers  <br/> |
|Called by:  <br/> |Client applications, the MAPI spooler, and MAPI  <br/> |
|Interface identifier:  <br/> |IID_IMsgStore  <br/> |
|Pointer type:  <br/> |LPMDB  <br/> |
|Transaction model:  <br/> |Nontransacted  <br/> |
   
## Vtable order

|Member |Description |
|:-----|:-----|
|[Advise](imsgstore-advise.md) <br/> |Registers to receive notification of specified events that affect the message store. |
|[Unadvise](imsgstore-unadvise.md) <br/> |Cancels the sending of notifications previously set up with a call to the **IMsgStore::Advise** method. |
|[CompareEntryIDs](imsgstore-compareentryids.md) <br/> |Compares two entry identifiers to determine whether they refer to the same entry in a message store. |
|[OpenEntry](imsgstore-openentry.md) <br/> |Opens a folder or message and returns an interface pointer for further access. |
|[SetReceiveFolder](imsgstore-setreceivefolder.md) <br/> |Establishes a folder as the destination for incoming messages of a particular message class. |
|[GetReceiveFolder](imsgstore-getreceivefolder.md) <br/> |Obtains the folder that was established as the destination for incoming messages of a specified message class or as the default receive folder for the message store. |
|[GetReceiveFolderTable](imsgstore-getreceivefoldertable.md) <br/> |Provides access to the receive folder table, a table with information about all of the receive folders for the message store. |
|[StoreLogoff](imsgstore-storelogoff.md) <br/> |Enables the orderly logoff of the message store. |
|[AbortSubmit](imsgstore-abortsubmit.md) <br/> |Attempts to remove a message from the outgoing queue. |
|[GetOutgoingQueue](imsgstore-getoutgoingqueue.md) <br/> |Provides access to the outgoing queue table, a table that has information about all of the messages in the message store's outgoing queue. |
|[SetLockState](imsgstore-setlockstate.md) <br/> |Locks or unlocks a message. |
|[FinishedMsg](imsgstore-finishedmsg.md) <br/> |Enables the message store provider to perform processing on a sent message. |
|[NotifyNewMail](imsgstore-notifynewmail.md) <br/> |Informs the message store that a new message has arrived. |
   
|**Required properties**|**Access level**|
|:-----|:-----|
|**PR_DISPLAY_NAME** ([PidTagDisplayName](pidtagdisplayname-canonical-property.md))  <br/> |Read/write  <br/> |
|**PR_ENTRYID** ([PidTagEntryId](pidtagentryid-canonical-property.md))  <br/> |Read-only  <br/> |
|**PR_OBJECT_TYPE** ([PidTagObjectType](pidtagobjecttype-canonical-property.md))  <br/> |Read-only  <br/> |
|**PR_RECORD_KEY** ([PidTagRecordKey](pidtagrecordkey-canonical-property.md))  <br/> |Read-only  <br/> |
|**PR_STORE_ENTRYID** ([PidTagStoreEntryId](pidtagstoreentryid-canonical-property.md))  <br/> |Read-only  <br/> |
|**PR_STORE_RECORD_KEY** ([PidTagStoreRecordKey](pidtagstorerecordkey-canonical-property.md))  <br/> |Read-only  <br/> |
|**PR_MDB_PROVIDER** ([PidTagStoreProvider](pidtagstoreprovider-canonical-property.md))  <br/> |Read-only  <br/> |
|**PR_STORE_SUPPORT_MASK** ([PidTagStoreSupportMask](pidtagstoresupportmask-canonical-property.md))  <br/> |Read-only  <br/> |
   
The following properties are for interpersonal message (IPM) message stores:
  
- **PR_IPM_OUTBOX_ENTRYID** ([PidTagIpmOutboxEntryId](pidtagipmoutboxentryid-canonical-property.md))
    
- **PR_IPM_SENTMAIL_ENTRYID** ([PidTagIpmSentMailEntryId](pidtagipmsentmailentryid-canonical-property.md))
    
- **PR_IPM_SUBTREE_ENTRYID** ([PidTagIpmSubtreeEntryId](pidtagipmsubtreeentryid-canonical-property.md))
    
- **PR_IPM_WASTEBASKET_ENTRYID** ([PidTagIpmWastebasketEntryId](pidtagipmwastebasketentryid-canonical-property.md))
    
- **PR_MDB_PROVIDER**
    
- **PR_STORE_SUPPORT_MASK**
    
## See also



[MAPI Properties](mapi-properties.md)

