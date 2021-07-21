---
title: "Get fileSecurityProfile"
description: "Read the properties and relationships of a fileSecurityProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get fileSecurityProfile
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [fileSecurityProfile](../resources/filesecurityprofile.md) object.

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
GET /security/fileSecurityProfiles/{fileSecurityProfileId}
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

If successful, this method returns a `200 OK` response code and a [fileSecurityProfile](../resources/filesecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_filesecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/fileSecurityProfiles/{fileSecurityProfileId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.fileSecurityProfile",
    "id": "074cb29f-b29f-074c-9fb2-4c079fb24c07",
    "activityGroupNames": [
      "String"
    ],
    "azureSubscriptionId": "String",
    "azureTenantId": "String",
    "certificateThumbprint": "String",
    "extensions": [
      "String"
    ],
    "fileType": "String",
    "firstSeenDateTime": "String (timestamp)",
    "hashes": [
      {
        "@odata.type": "microsoft.graph.fileHash"
      }
    ],
    "lastSeenDateTime": "String (timestamp)",
    "malwareStates": [
      {
        "@odata.type": "microsoft.graph.malwareState"
      }
    ],
    "names": [
      "String"
    ],
    "riskScore": "String",
    "size": "Integer",
    "tags": [
      "String"
    ],
    "vendorInformation": {
      "@odata.type": "microsoft.graph.securityVendorInformation"
    },
    "vulnerabilityStates": [
      {
        "@odata.type": "microsoft.graph.vulnerabilityState"
      }
    ]
  }
}
```
