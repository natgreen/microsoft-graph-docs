---
title: "macOSKerberosSingleSignOnExtension resource type"
description: "Represents a Kerberos-type Single Sign-On extension profile for macOS devices."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# macOSKerberosSingleSignOnExtension resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a Kerberos-type Single Sign-On extension profile for macOS devices.


Inherits from [macOSSingleSignOnExtension](../resources/macossinglesignonextension.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeDirectorySiteCode|String|Gets or sets the Active Directory site.|
|blockActiveDirectorySiteAutoDiscovery|Boolean|Enables or disables whether the Kerberos extension can automatically determine its site name.|
|blockAutomaticLogin|Boolean|Enables or disables Keychain usage.|
|cacheName|String|Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile.|
|credentialBundleIdAccessControlList|String collection|Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket.|
|domainRealms|String collection|Gets or sets a list of realms for custom domain-realm mapping. Realms are case sensitive.|
|domains|String collection|Gets or sets a list of hosts or domain names for which the app extension performs SSO.|
|isDefaultRealm|Boolean|When true, this profile's realm will be selected as the default. Necessary if multiple Kerberos-type profiles are configured.|
|passwordBlockModification|Boolean|Enables or disables password changes.|
|passwordChangeUrl|String|Gets or sets the URL that the user will be sent to when they initiate a password change.|
|passwordEnableLocalSync|Boolean|Enables or disables password syncing. This won't affect users logged in with a mobile account on macOS.|
|passwordExpirationDays|Int32|Overrides the default password expiration in days. For most domains, this value is calculated automatically.|
|passwordExpirationNotificationDays|Int32|Gets or sets the number of days until the user is notified that their password will expire (default is 15).|
|passwordMinimumAgeDays|Int32|Gets or sets the minimum number of days until a user can change their password again.|
|passwordMinimumLength|Int32|Gets or sets the minimum length of a password.|
|passwordPreviousPasswordBlockCount|Int32|Gets or sets the number of previous passwords to block.|
|passwordRequireActiveDirectoryComplexity|Boolean|Enables or disables whether passwords must meet Active Directory's complexity requirements.|
|passwordRequirementsDescription|String|Gets or sets a description of the password complexity requirements.|
|realm|String|Gets or sets the case-sensitive realm name for this profile.|
|requireUserPresence|Boolean|Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry.|
|userPrincipalName|String|Gets or sets the principle user name to use for this profile. The realm name does not need to be included.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKerberosSingleSignOnExtension",
  "activeDirectorySiteCode": "String",
  "blockActiveDirectorySiteAutoDiscovery": "Boolean",
  "blockAutomaticLogin": "Boolean",
  "cacheName": "String",
  "credentialBundleIdAccessControlList": [
    "String"
  ],
  "domainRealms": [
    "String"
  ],
  "domains": [
    "String"
  ],
  "isDefaultRealm": "Boolean",
  "passwordBlockModification": "Boolean",
  "passwordChangeUrl": "String",
  "passwordEnableLocalSync": "Boolean",
  "passwordExpirationDays": "Integer",
  "passwordExpirationNotificationDays": "Integer",
  "passwordMinimumAgeDays": "Integer",
  "passwordMinimumLength": "Integer",
  "passwordPreviousPasswordBlockCount": "Integer",
  "passwordRequireActiveDirectoryComplexity": "Boolean",
  "passwordRequirementsDescription": "String",
  "realm": "String",
  "requireUserPresence": "Boolean",
  "userPrincipalName": "String"
}
```
