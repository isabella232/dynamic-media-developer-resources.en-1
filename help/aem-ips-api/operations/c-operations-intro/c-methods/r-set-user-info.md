---
description: Sets user attributes (e.g., name, email, role, etc.)
solution: Experience Manager
title: setUserInfo
feature: Dynamic Media Classic,SDK/API
role: Developer,Admin
exl-id: d8f8fe53-a874-4b77-9084-9a369862a672
---
# setUserInfo{#setuserinfo}

Sets user attributes (e.g., name, email, role, etc.)

 Syntax 

## Authorized User Types {#section-6c28db5d15b3449492a73749e4f981ac}

* `IpsAdmin` 
* `IpsCompanyAdmin` 
* `TrialSiteAdmin` 
* `ImagePortalAdmin`

## Parameters {#section-71b457921fe74acb862a1e112e550211}

**Input (setUserInfoParam)** 

|  Name  | Type  | Required  | Description  |
|---|---|---|---|
|  userHandle  | `xsd:string`  | No  | User handle.  |
|  firstName  | `xsd:string`  | Yes  | First name.  |
|  lastName  | `xsd:string`  | Yes  | Last name.  |
|  email  | `xsd:string`  | Yes  | User email.  |
|  defaultRole  | `xsd:string`  | Yes  |Sets the role for a user in each company they belong to. Note, however, the `IpsAdmin` role overrides other per-company settings.  |
|  passwordExpires  | `xsd:dateTime`  | No  | Set's password expiration date.  |
|  isValid  | `xsd:boolean`  | Yes  | Determines if user is a valid IPS user.  |
|  membershipArray  | `types:CompanyMembershipUpdateArray`  | Yes  | An array of company handles.  |

**Output (setUserInfoReturn)**

The IPS API does not return a response for this operation.

## Examples {#section-272c103076fb4de0a53729e2f6bfb895}

**Request** 

```java
<setUserInfoParam xmlns="http://www.scene7.com/IpsApi/xsd">
   <firstName>test</firstName>
   <lastName>test</lastName>
   <email>test@test.test</email>
   <defaultRole>IpsAdmin</defaultRole>
   <isValid>true</isValid>
</setUserInfoParam>
```

**Response**

None.
