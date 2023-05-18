---
title: "current element (weatherType complexType) (Outlook Weather Information Schema)"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.service: office-online-server
ms.localizationpriority: medium
ms.assetid: d592a396-f935-c44c-409f-b849c327cfbd
description: "Specifies the current weather conditions."
---

# current element (weatherType complexType) (Outlook Weather Information Schema)

Specifies the current weather conditions.
  
## Element information

|Property |Value |
|:-----|:-----|
|**Element type** <br/> |[currentType](currenttype-complextype-outlook-weather-information-schema.md) <br/> |
|**Namespace** <br/> |http://schemas.microsoft.com/office/outlook/15/getweatherinfo.xsd  <br/> |
|**Schema file** <br/> |getweatherinfo.xsd  <br/> |
   
## Definition

```XML
<xs:element name="current"      type="currentType">
  </xs:element>  

```

## Elements and attributes

If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section. 
  
### Parent elements

|**Element**|**Type**|**Description**|
|:-----|:-----|:-----|
|[weather](weather-element-weatherdata-elementoutlook-weather-information-schema.md) <br/> |[weatherType](weathertype-complextype-outlook-weather-information-schema.md) <br/> |Specifies the weather conditions of a location. |
   
### Child elements

None.
  
### Attributes

|**Attribute**|**Type**|**Required**|**Description**|**Possible values**|
|:-----|:-----|:-----|:-----|:-----|
|date  <br/> |xs:date  <br/> |required  <br/> |Specifies today's date. |A value of the type xs:date  <br/> |
|day  <br/> |xs:string  <br/> |optional  <br/> |Specifies a day for the forecast. |A value of the type xs:string  <br/> |
|feelslike  <br/> |xs:integer  <br/> |required  <br/> |Specifies the temperature of how the current weather feels like. |A value of the type xs:integer  <br/> |
|humidity  <br/> |xs:integer  <br/> |required  <br/> |Specifies the current numerical humidity value. |A value of the type xs:integer  <br/> |
|observationpoint  <br/> |xs:string  <br/> |required  <br/> |Specifies where the current weather information is observed from. |A value of the type xs:string  <br/> |
|observationtime  <br/> |xs:time  <br/> |required  <br/> |Specifies when the current weather information is observed at. |A value of the type xs:time  <br/> |
|shortday  <br/> |xs:string  <br/> |optional  <br/> |Specifies a day in abbreviated form. |A value of the type xs:string  <br/> |
|skycode  <br/> |xs:integer  <br/> |required  <br/> |Specifies an integer code for the current weather conditions. |A value of the type xs:integer  <br/> |
|skytext  <br/> |xs:string  <br/> |required  <br/> |Specifies one to two words describing current weather conditions. |A value of the type xs:string  <br/> |
|temperature  <br/> |xs:integer  <br/> |required  <br/> |Specifies the current temperature of the location. |A value of the type xs:integer  <br/> |
|winddisplay  <br/> |xs:string  <br/> |required  <br/> |A string that describes the current wind conditions. |A value of the type xs:string  <br/> |
|windspeed  <br/> |xs:integer  <br/> |required  <br/> |Specifies the current numerical wind speed value. |A value of the type xs:integer  <br/> |
   

