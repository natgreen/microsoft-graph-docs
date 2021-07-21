---
title: "Get androidCompliancePolicy"
description: "Read the properties and relationships of an androidCompliancePolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get androidCompliancePolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [androidCompliancePolicy](../resources/androidcompliancepolicy.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Entity URI for microsoft.graph.androidCompliancePolicy not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [androidCompliancePolicy](../resources/androidcompliancepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_androidcompliancepolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.graph.androidCompliancePolicy not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidCompliancePolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCompliancePolicy",
    "id": "91e9512c-512c-91e9-2c51-e9912c51e991",
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "displayName": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "roleScopeTagIds": [
      "String"
    ],
    "version": "Integer",
    "advancedThreatProtectionRequiredSecurityLevel": "String",
    "conditionStatementId": "String",
    "deviceThreatProtectionEnabled": "Boolean",
    "deviceThreatProtectionRequiredSecurityLevel": "String",
    "minAndroidSecurityPatchLevel": "String",
    "osMaximumVersion": "String",
    "osMinimumVersion": "String",
    "passwordExpirationDays": "Integer",
    "passwordMinimumLength": "Integer",
    "passwordMinutesOfInactivityBeforeLock": "Integer",
    "passwordPreviousPasswordBlockCount": "Integer",
    "passwordRequired": "Boolean",
    "passwordRequiredType": "String",
    "passwordSignInFailureCountBeforeFactoryReset": "Integer",
    "requiredPasswordComplexity": "String",
    "restrictedApps": [
      {
        "@odata.type": "microsoft.graph.appListItem"
      }
    ],
    "securityBlockDeviceAdministratorManagedDevices": "Boolean",
    "securityBlockJailbrokenDevices": "Boolean",
    "securityDisableUsbDebugging": "Boolean",
    "securityPreventInstallAppsFromUnknownSources": "Boolean",
    "securityRequireCompanyPortalAppIntegrity": "Boolean",
    "securityRequireGooglePlayServices": "Boolean",
    "securityRequireSafetyNetAttestationBasicIntegrity": "Boolean",
    "securityRequireSafetyNetAttestationCertifiedDevice": "Boolean",
    "securityRequireUpToDateSecurityProviders": "Boolean",
    "securityRequireVerifyApps": "Boolean",
    "storageRequireEncryption": "Boolean"
  }
}
```
