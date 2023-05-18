---
title: "XML for friends"
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: overview
ms.service: office-online-server
ms.localizationpriority: medium
ms.assetid: 3362639a-8098-47ab-ba94-ee89e4920032
description: "The friends element in the Microsoft Outlook Social Connector (OSC) provider XML schema allows an OSC provider to specify information for a list of persons associated with an Outlook user in the social network."
---

# XML for friends

The **friends** element in the Microsoft Outlook Social Connector (OSC) provider XML schema allows an OSC provider to specify information for a list of persons associated with an Outlook user in the social network. If the OSC provider supports cached synchronization, this list of person will contain only friends of the Outlook user on the social network. If the OSC supports on-demand or hybrid synchronization, this list may contain both friends and non-friends of the Outlook user. 

Each person in the list is represented as a **person** element in the XML schema, which supports details such as first name, last name, and email addresses. OSC providers use the **friends** and **person** elements regardless of how they want the OSC to synchronize friend information from the social network. Note that the child elements of **person** are similar to some of the properties of an Outlook contact, which facilitates storing friends in an Outlook contacts folder specific to the social network, if the social network supports cached or hybrid synchronization of friends to an Outlook contacts folder. 

## Example scenarios

The following example scenarios show the OSC provider extensibility API calls that an OSC provider implements and the OSC makes to obtain friend information. Information is expressed in XML strings that conform to the OSC provider XML schema.
  
For an example of friends XML, see [Friends XML Example](friends-xml-example.md). For more information about synchronizing friends' information, see [Synchronizing Friends and Activities](synchronizing-friends-and-activities.md).

### Scenario 1: get a list of friends

Scenario 1—OSC gets a list of friends, and an [ISocialPerson](isocialpersoniunknown.md) object and a picture for each friend: 
    
1. An OSC provider that supports showing friends from the social network site and allowing the OSC to cache friend information indicates that to the OSC by using the **getFriends** and **cacheFriends** elements, which are child elements of the **capabilities** element. 
    
2. The OSC provider also implements the [ISocialProvider::GetCapabilities](isocialprovider-getcapabilities.md), [ISocialSession::GetPerson](isocialsession-getperson.md), [ISocialPerson::GetFriendsAndColleagues](isocialperson-getfriendsandcolleagues.md), and [ISocialPerson::GetPicture](isocialperson-getpicture.md) methods. 
    
3. The OSC calls **ISocialProvider::GetCapabilities** to check the value of the following elements: **getFriends** to verify that the OSC provider supports showing friends from the social network, and **cacheFriends** to verify that the provider supports caching friends. 
    
4. The OSC calls **ISocialSession::GetPerson** to get an **ISocialPerson** object for the Outlook user. 
    
5. The OSC calls **ISocialPerson::GetFriendsAndColleagues** to get the Outlook user's friends list returned in the _personCollection_ parameter string. The  _personCollection_ string complies with the XML schema definition for the **friends** element in the XML schema. 
    
6. For each friend in the _personCollection_ XML string, the OSC obtains value of the **userID** element to call **ISocialSession::GetPerson** to get an **ISocialPerson** object for that friend. 
    
7. For each friend in the **personCollection** XML string, the OSC calls [ISocialPerson::GetPicture](isocialperson-getpicture.md) to get a picture resource for that friend. 
    
   The OSC can make further calls on the **ISocialPerson** object to obtain activities and details (for example, email addresses) for that friend. 
    
### Scenario 2: synchronize friends 

Scenario 2—OSC synchronizes friends dynamically:
    
1. An OSC provider that supports on-demand synchronization of friends and non-friends indicates that to the OSC by using the **getFriends** and **dynamicContactsLookup** elements. The OSC provider also sets the **hashFunction** element. All three elements are child elements of **capabilities**. 
    
2. The OSC provider also implements the [ISocialSession2::GetPeopleDetails](isocialsession2-getpeopledetails.md) method. 
    
3. The OSC calls **ISocialProvider::GetCapabilities** to check the values of **getFriends** and **dynamicContactsLookup** to verify that the OSC provider supports friends and on-demand synchronization of friends and non-friends. The OSC also makes note of the value of **hashFunction** supported by the OSC provider. 
    
4. For each user displayed in the People Pane, the OSC collects the user's email address and encrypts it by using the hash function specified in **hashFunction**. This forms an XML string that conforms to the XML schema definition for the **hashedAddresses** element. 
    
5. The OSC calls **ISocialSession2::GetPeopleDetails**, providing this XML string of hashed addresses as the  _personAddresses_ parameter, to dynamically obtain updated details for persons in the _personsCollection_ parameter. The  _personsCollection_ parameter string complies with the XML schema definition for the **friends** element in the XML schema. 

## Parent and child elements

The following are the two top-level elements in the **friends** schema. 
  
|**Element**|**Description**|
|:-----|:-----|
|**friends** <br/> |Represents the root element of a list of **person** elements. The **ISocialPerson::GetFriendsAndColleagues**, [ISocialSession::FindPerson](isocialsession-findperson.md), and **ISocialSession2::GetPeopleDetails** return XML strings that conform to the schema definition of the **friends** element. |
|**person** <br/> |Represents one person in a list of **person** elements. The [ISocialPerson::GetDetails](isocialperson-getdetails.md) method returns an XML string that conforms to the schema definition of the **person** element. |
   
The following table describes each child element of the **person** element in the OSC provider XML schema. 
  
For a complete definition of the OSC provider XML schema, including which elements are required or optional, see [Outlook Social Connector Provider XML Schema](outlook-social-connector-provider-xml-schema.md).
  
|**Element**|**Description**|
|:-----|:-----|
|**address** <br/> |Physical street address of the person. |
|**anniversary** <br/> |Anniversary date for an event for the person. |
|**askmeabout** <br/> |Topics of interest or expertise of the person. |
|**birthday** <br/> |Date of birth for the person. |
|**businessAddress** <br/> |Physical street address of the person's workplace. |
|**businessCity** <br/> |City for the person's workplace. |
|**businessCountryOrRegion** <br/> |Country or region of the person's workplace. |
|**businessState** <br/> |State or province of the person's workplace. |
|**businessZip** <br/> |Zip or postal code of the person's workplace. |
|**cell** <br/> |Mobile telephone number for the person. |
|**city** <br/> |City of the physical address for the person. |
|**company** <br/> |Name of the company associated with the person. |
|**countryOrRegion** <br/> |Country or region of the physical address of the person. |
|**creationTime** <br/> |Creation time of the person's profile on the social network. |
|**emailAddress** <br/> |Primary email address of the person. |
|**emailAddress2** <br/> |Secondary email address of the person. |
|**emailAddress3** <br/> |Tertiary email address of the person. |
|**expirationTime** <br/> |Time that the person's profile data expires on the social network. |
|**fileAs** <br/> |String by which the person is to be filed as a contact in an Outlook contacts file. |
|**firstName** <br/> |First name or given name of the person. |
|**friendStatus** <br/> |Friend status of this person with the logged on user on the social network. Must be one of the following values: **friend**, **nonfriend**, **pending**, **pendingin**, **pendingout**. |
|**fullName** <br/> |Full name of the person. |
|**gender** <br/> |Gender of the person. Must be one of the following values: **male**, **female**, **unspecified**. |
|**homePhone** <br/> |Home telephone number for the person. |
|**index** <br/> |Location of the person's hashed address in the _personsAddresses_ string parameter passed to a call to the **ISocialSession2::GetPeopleDetails** method. It also indicates the person's **person** XML in the _personsCollection_ string returned by **GetPeopleDetails**. |
|**industries** <br/> |Industries that the person is engaged in. |
|**interests** <br/> |Interests or hobbies of the person. |
|**lastModificationTime** <br/> |Time that the person's profile was last modified on the social network. |
|**lastName** <br/> |Last name or surname of the person. |
|**location** <br/> |The location of the person. |
|**nickname** <br/> |A shorter name or invented name of the person. |
|**otherAddress** <br/> |Alternative street address of the person. |
|**otherCity** <br/> |City of the person's alternative address. |
|**otherCountryOrRegion** <br/> |Country or region of the person's alternative address. |
|**otherState** <br/> |State or province of the person's alternative address. |
|**otherZip** <br/> |Zip or postal code of the person's alternative address. |
|**phone** <br/> |Primary contact telephone number for the person. |
|**pictureUrl** <br/> |URL for a profile picture of the person. |
|**relationship** <br/> |Relationship of this person with the logged on user. |
|**schools** <br/> |The schools that the person goes or went to. |
|**skills** <br/> |Personal skills of the person. |
|**state** <br/> |State or province of the physical address of the person. |
|**title** <br/> |Designation added to the person's name. |
|**userID** <br/> |ID to identify the person on the social network. |
|**webProfilePage** <br/> |Webpage address that contains a profile of the person. |
|**website** <br/> |The person's web site. |
|**workPhone** <br/> |Business telephone number for the person. |
|**zip** <br/> |ZIP code or postal code of the physical address of the person. |
   
## See also

- [Friends XML Example](friends-xml-example.md)  
- [Synchronizing Friends and Activities](synchronizing-friends-and-activities.md)  
- [XML for Capabilities](xml-for-capabilities.md) 
- [XML for Activities](xml-for-activities.md)
- [Developing a Provider with the OSC XML Schema](developing-a-provider-with-the-osc-xml-schema.md)

