---
title: "Issue_Type complexType (Visio XML)"
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: d6768062-37aa-5658-f068-dae8d3a24717

---

# Issue_Type complexType (Visio XML)

## Type information

| Type | Info |
| :------------------------|:----------------------------------|
| **Namespace** <br/>      | `http://schemas.microsoft.com/office/visio/2011/1/core`  <br/> |
| **Schema file** <br/>    | VisioSchema15-2012-06-05.xsd  <br/> |
| **Extension base** <br/> | None  <br/> |
   
## Definition

```XML
          <xs:complexType name="Issue_Type">
          
          <xs:sequence>
    <xs:element name="IssueTarget"  type="IssueTarget_Type"
     minOccurs="0"
     maxOccurs="1"
    >
    </xs:element>
    
    <xs:element name="RuleInfo"  type="RuleInfo_Type"
     minOccurs="0"
     maxOccurs="1"
    >
    </xs:element>
    
      </xs:sequence>
    <xs:attribute name="ID"
  type="xsd:unsignedInt"
     use="required"
    />
    <xs:attribute name="Ignored"
  type="xsd:boolean"
    />
      </xs:complexType>
      
```

## Elements and attributes

If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section. 
  
### Child elements

| Element | Type |
|:----------|:-------|
|[IssueTarget](issuetarget-element-issue_type-complextypevisio-xml.md) <br/> | [IssueTarget_Type](issuetarget_type-complextypevisio-xml.md) <br/> |
|[RuleInfo](ruleinfo-element-issue_type-complextypevisio-xml.md) <br/>       | [RuleInfo_Type](ruleinfo_type-complextypevisio-xml.md) <br/> |
   
### Attributes

| Attribute      | Type                   | Required        | Possible values    |
| :--------------| :----------------------| :---------------| :------------------|
| ID  <br/>      | xsd:unsignedInt <br/>  | required <br/>  | Values of the xsd:unsignedInt type. |
| Ignored <br/>  | xsd:boolean <br/>      | optional <br/>  | Values of the xsd:boolean type. |
   
### See also
[Introduction to the Visio file format (.vsdx)](/office/client-developer/visio/introduction-to-the-visio-file-formatvsdx)
