---
title: "Get deviceEnrollmentWindowsHelloForBusinessConfiguration"
description: "Read the properties and relationships of a deviceEnrollmentWindowsHelloForBusinessConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get deviceEnrollmentWindowsHelloForBusinessConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) object.

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
GET ** Entity URI for microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration not found
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

If successful, this method returns a `200 OK` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_deviceenrollmentwindowshelloforbusinessconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
    "id": "1030f956-f956-1030-56f9-301056f93010",
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "displayName": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "priority": "Integer",
    "roleScopeTagIds": [
      "String"
    ],
    "version": "Integer",
    "enhancedBiometricsState": "String",
    "pinExpirationInDays": "Integer",
    "pinLowercaseCharactersUsage": "String",
    "pinMaximumLength": "Integer",
    "pinMinimumLength": "Integer",
    "pinPreviousBlockCount": "Integer",
    "pinSpecialCharactersUsage": "String",
    "pinUppercaseCharactersUsage": "String",
    "remotePassportEnabled": "Boolean",
    "securityDeviceRequired": "Boolean",
    "securityKeyForSignIn": "String",
    "state": "String",
    "unlockWithBiometricsEnabled": "Boolean"
  }
}
```
