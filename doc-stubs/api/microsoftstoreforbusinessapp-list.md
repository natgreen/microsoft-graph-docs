---
title: "List microsoftStoreForBusinessApps"
description: "Get a list of the microsoftStoreForBusinessApp objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List microsoftStoreForBusinessApps
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.microsoftStoreForBusinessApp not found
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

If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessApp](../resources/microsoftstoreforbusinessapp.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_microsoftstoreforbusinessapp"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.microsoftStoreForBusinessApp not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.microsoftStoreForBusinessApp)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
      "id": "fb111d3c-1d3c-fb11-3c1d-11fb3c1d11fb",
      "createdDateTime": "String (timestamp)",
      "dependentAppCount": "Integer",
      "description": "String",
      "developer": "String",
      "displayName": "String",
      "informationUrl": "String",
      "isAssigned": "Boolean",
      "isFeatured": "Boolean",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "notes": "String",
      "owner": "String",
      "privacyInformationUrl": "String",
      "publisher": "String",
      "publishingState": "String",
      "roleScopeTagIds": [
        "String"
      ],
      "supersededAppCount": "Integer",
      "supersedingAppCount": "Integer",
      "uploadState": "Integer",
      "licenseType": "String",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType"
      },
      "packageIdentityName": "String",
      "productKey": "String",
      "totalLicenseCount": "Integer",
      "usedLicenseCount": "Integer"
    }
  ]
}
```
