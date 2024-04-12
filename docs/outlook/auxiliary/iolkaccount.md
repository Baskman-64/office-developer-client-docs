---
title: "IOlkAccount"
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 7b7cb295-fc77-a8b9-aac9-e548f3b4afcb
---

# IOlkAccount

Supports getting and setting of properties and other information about an account.
  
## Quick info

|Property |Value |
|:-----|:-----|
|Inherits from:  <br/> |[IOlkErrorUnknown](iolkerrorunknown.md) <br/> |
|Implemented by:  <br/> |Outlook  <br/> |
|Provided by:  <br/> |[IOlkAccountManager::FindAccount](iolkaccountmanager-findaccount.md) and [IOlkEnum::GetNext](iolkenum-getnext.md) <br/> |
|Called by:  <br/> |Client  <br/> |
|Interface identifier:  <br/> |IID_IOlkAccount  <br/> |
   
## Vtable order

|Member |Description |
|:-----|:-----|
| *Placeholder member*  <br/> | *Not supported or documented.*  <br/> |
| *Placeholder member*  <br/> | *Not supported or documented.*  <br/> |
| *Placeholder member*  <br/> | *Not supported or documented.*  <br/> |
| *Placeholder member*  <br/> | *Not supported or documented.*  <br/> |
| *Placeholder member*  <br/> | *Not supported or documented.*  <br/> |
| *Placeholder member*  <br/> | *Not supported or documented.*  <br/> |
|[GetAccountInfo](iolkaccount-getaccountinfo.md) <br/> |Gets the type and categories of the specified account. |
|[GetProp](iolkaccount-getprop.md) <br/> |Gets the value of the specified account property. See the Properties table below. |
|[SetProp](iolkaccount-setprop.md) <br/> |Sets the value of the specified account property. See the Properties table below. |
| *Placeholder member*  <br/> | *Not supported or documented.*  <br/> |
| *Placeholder member*  <br/> | *Not supported or documented.*  <br/> |
| *Placeholder member*  <br/> | *Not supported or documented.*  <br/> |
|[FreeMemory](iolkaccount-freememory.md) <br/> |Frees memory allocated by the **IOlkAccount** interface. |
| *Placeholder member*  <br/> | *Not supported or documented.*  <br/> |
|[SaveChanges](iolkaccount-savechanges.md) <br/> |Commits changes to the account object by writing to the registry store. |
   
## Properties

|Property |Value |
|:-----|:-----|
|[PROP_ACCT_DELIVERY_FOLDER](prop_acct_delivery_folder.md) <br/> |Represents the Entry ID of the default delivery folder for the account. |
|[PROP_ACCT_DELIVERY_STORE](prop_acct_delivery_store.md) <br/> |Represents the Entry ID of the default delivery store for the account. |
|[PROP_ACCT_ID](prop_acct_id.md) <br/> |Returns the account identifier in Outlook 2000 and earlier versions of Outlook. |
|[PROP_ACCT_IS_EXCH](prop_acct_is_exch.md) <br/> |True if the account is a Microsoft Exchange account. |
|[PROP_ACCT_MINI_UID](prop_acct_mini_uid.md) <br/> |Returns the account identifier in versions of Outlook since Outlook 2002. |
|[PROP_ACCT_NAME](prop_acct_name.md) <br/> |Returns the account name. |
|[PROP_ACCT_PREFERENCES_UID](prop_acct_preferences_uid.md) <br/> |Retrieves the unique identifier (UID) for the profile section that stores the account preferences. |
|[PROP_ACCT_SEND_STAMP](prop_acct_send_stamp.md) <br/> |Returns the account "send" stamp. |
|[PROP_ACCT_SENTITEMS_EID](prop_acct_sentitems_eid.md) <br/> |Represents the Entry ID of the default folder for sent items for the account. |
|[PROP_ACCT_STAMP](prop_acct_stamp.md) <br/> |Returns the account stamp. |
|[PROP_ACCT_USER_DISPLAY_NAME](prop_acct_user_display_name.md) <br/> |Returns the user display name. |
|[PROP_ACCT_USER_EMAIL_ADDR](prop_acct_user_email_addr.md) <br/> |Specifies the email address for the account. |
|[PROP_MAPI_EMSMDB_UID](prop_mapi_emsmdb_uid.md) <br/> |Represents an [ACCT_BIN](acct_bin.md) structure that contains the UID of an Exchange account. |
|[PROP_MAPI_IDENTITY_ENTRYID](prop_mapi_identity_entryid.md) <br/> |Retrieves or sets the address book entry ID for the account. |
|[PROP_MAPI_TRANSPORT_FLAGS](prop_mapi_transport_flags.md) <br/> |Represents transport settings that Microsoft Outlook uses to determine the necessary synchronization tasks and to disable the user interface (UI) elements that the account does not support. |
   
## Remarks

This interface is returned by **IOlkAccountManager::FindAccount** when searching for an account that supports **IOlkAccount** and **IOlkEnum::GetNext** when getting the next account in an enumerator. 
  
## See also

- [About the Account Management API](about-the-account-management-api.md)  
- [Constants (Account management API)](constants-account-management-api.md)

