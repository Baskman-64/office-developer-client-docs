---
title: "PageSheet element (Master_Type complexType) (Visio XML)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
 
ms.localizationpriority: medium
ms.assetid: 824fbeb0-1a2f-35a0-50e3-c57143dc21ab
description: "Specifies the properties of the drawing page associated with the master."
---

# PageSheet element (Master_Type complexType) (Visio XML)

Specifies the properties of the drawing page associated with the master.
  
## Element information

||Value |
|:-----|:-----|
|**Element type** <br/> |[PageSheet_Type](pagesheet_type-complextypevisio-xml.md) <br/> |
|**Namespace** <br/> |http://schemas.microsoft.com/office/visio/2012/main  <br/> |
|**Schema file** <br/> |VisioSchema15.xsd  <br/> |
|**Document parts** <br/> |masters.xml  <br/> |
   
## Definition

```XML
< xs:element name="PageSheet" type="PageSheet_Type" minOccurs="0" maxOccurs="1" >
</xs:element >
```

## Elements and attributes

If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section. 
  
### Parent elements

|**Element**|**Type**|**Description**|
|:-----|:-----|:-----|
|[Master](master-element-masters_type-complextypevisio-xml.md) <br/> |[Master_Type](master_type-complextypevisio-xml.md) <br/> |Specifies a master in a drawing. |
   
### Child elements

None.
  
### Attributes

|**Attribute**|**Type**|**Required**|**Description**|**Possible values**|
|:-----|:-----|:-----|:-----|:-----|
|FillStyle  <br/> |xsd:unsignedInt  <br/> |optional  <br/> |specifies the ID of the style sheet from which to inherit fill formatting. It MUST be the value of the **ID** attribute associated with a **StyleSheet_Type** in the drawing. |Values of the xsd:unsignedInt type. |
|LineStyle  <br/> |xsd:unsignedInt  <br/> |optional  <br/> |Specifies the ID of the style sheet from which to inherit line formatting. It MUST be the value of the **ID** attribute associated with a **StyleSheet_Type** in the drawing. |Values of the xsd:unsignedInt type. |
|TextStyle  <br/> |xsd:unsignedInt  <br/> |optional  <br/> |Specifies the ID of the style sheet from which to inherit text formatting. It MUST be the value of the **ID** attribute associated with a **StyleSheet_Type** in the drawing. |Values of the xsd:unsignedInt type. |
|UniqueID  <br/> |xsd:string  <br/> |optional  <br/> |The unique ID of the element within its parent element. |Values of the xsd:string type. |
   

