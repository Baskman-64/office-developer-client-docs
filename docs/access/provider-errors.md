---
title: "Provider Errors"
 
 
manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
  
localization_priority: Normal
ms.assetid: 9c39d450-6e67-b2fd-aeb5-849e6b65fd54
description: "When a provider error occurs, a run-time error of -2147467259 is returned. When you receive this error, check the active Connection object's Errors collection, which will contain one or more errors describing what happened."
---

# Provider Errors

When a provider error occurs, a run-time error of -2147467259 is returned. When you receive this error, check the active **Connection** object's **Errors** collection, which will contain one or more errors describing what happened. 
  
## The ADO Errors Collection

Because a particular ADO operation can produce multiple provider errors, ADO exposes a collection of error objects through the **Connection** object. This collection contains no objects if an operation concludes successfully and contains one or more **Error** objects if something went wrong and the provider raised one or more errors. Examine each individual error object in order to determine the exact cause of the error. 
  
Once you have finished handling any errors that have occurred, you can clear the collection by calling the **Clear** method. It is particularly important to explicitly clear the **Errors** collection before you call the **Resync**, **UpdateBatch**, or **CancelBatch** method on a **Recordset** object, the **Open** method on a **Connection** object, or set the **Filter** property on a **Recordset** object. By clearing the collection explicitly, you can be certain that any **Error** objects in the collection are not left over from a previous operation. 
  
Some operations can generate warnings as well as errors. Warnings are also represented by **Error** objects in the **Errors** collection. When a provider adds a warning to the collection, it does not generate a run-time error. Check the **Count** property of the **Errors** collection to determine if a warning was produced by a particular operation. If the count is one or greater, an **Error** object has been added to the collection. Once you have determined that the **Errors** collection contains errors or warnings, you can iterate through the collection and retrieve information about each of the **Error** objects it contains. The following short Visual Basic example demonstrates this: 
  
```
 
' BeginErrorHandlingVB02 
Private Function DeleteCustomer(ByVal CompanyName As String) As Long 
 On Error GoTo DeleteCustomerError 
 
 rst.Find "CompanyName='" &amp; CompanyName &amp; "'" 
 
DeleteCustomerError: 
 
 Dim objError As ADODB.Error 
 Dim strError As String 
 
 If cnn.Errors.Count > 0 Then 
 For Each objError In cnn.Errors 
 strError = strError &amp; "Error #" &amp; objError.Number &amp; _ 
 " " &amp; objError.Description &amp; vbCrLf &amp; _ 
 "NativeError: " &amp; objError.NativeError &amp; vbCrLf &amp; _ 
 "SQLState: " &amp; objError.SQLState &amp; vbCrLf &amp; _ 
 "Reported by: " &amp; objError.Source &amp; vbCrLf &amp; _ 
 "Help file: " &amp; objError.HelpFile &amp; vbCrLf &amp; _ 
 "Help Context ID: " &amp; objError.HelpContext 
 Next 
 MsgBox strError 
 End If 
End Function 
' EndErrorHandlingVB02 

```

The error-handling routine includes a **For Each** loop that examines each object in the **Errors** collection. In this example, it simply accumulates a message for display. In a working program, you would write code to perform an appropriate task for each error, such as closing all open files and shutting down the program in an orderly fashion. 
  
## The Error Object

By examining an **Error** object you can determine what error occurred, and more importantly, what application or what object caused the error. The **Error** object has the following properties: 
  
|**Property name**|**Description**|
|:-----|:-----|
|**Description** <br/> |A text description of the error that occurred.  <br/> |
|**HelpContext, HelpFile** <br/> |Refers to the help topic and help file that contain a description of the error that occurred.  <br/> |
|**NativeError** <br/> |The provider-specific error number.  <br/> |
|**Number** <br/> |A Long Integer that represents the number (listed in the **ErrorValueEnum** ) of the error that occurred.  <br/> |
|**Source** <br/> |Indicates the name of the object or application that generated an error.  <br/> |
|**SQLState** <br/> |A five-character error code that the provider returns during the process of a SQL statement.  <br/> |
   
The ADO **Error** object is quite similar to the standard Visual Basic **Err** object. Its properties describe the error that occurred. In addition to the number of the error, you also receive two related pieces of information. The **NativeError** property contains an error number specific to the provider you are using. In the previous example, the provider is the Microsoft OLE DB Provider for SQL Server, so **NativeError** will contain errors specific to SQL Server. The **SQLState** property has a five-letter code that describes an error in a SQL statement. 
  
## Event-Related Errors

The **Error** object is also used when event-related errors occur. You can determine if an error occurred in the process that raised an ADO event by checking the **Error** object passed as an event parameter. 
  
If the operation that causes an event is concluded successfully, the  *adStatus*  parameter of the event handler will be set to  *adStatusOK*  . On the other hand, if the operation that raised the event was unsuccessful, the  *adStatus*  parameter is set to  *adStatusErrorsOccurred*  . In that case, the  *pError*  parameter will contain an **Error** object that describes the error. 
  
