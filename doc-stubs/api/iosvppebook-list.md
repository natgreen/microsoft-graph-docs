---
title: "List iosVppEBooks"
description: "Get a list of the iosVppEBook objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List iosVppEBooks
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [iosVppEBook](../resources/iosvppebook.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.iosVppEBook not found
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

If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/iosvppebook.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_iosvppebook"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.iosVppEBook not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.iosVppEBook)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBook",
      "id": "82097bae-7bae-8209-ae7b-0982ae7b0982",
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "displayName": "String",
      "informationUrl": "String",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "privacyInformationUrl": "String",
      "publishedDateTime": "String (timestamp)",
      "publisher": "String",
      "appleId": "String",
      "genres": [
        "String"
      ],
      "language": "String",
      "roleScopeTagIds": [
        "String"
      ],
      "seller": "String",
      "totalLicenseCount": "Integer",
      "usedLicenseCount": "Integer",
      "vppOrganizationName": "String",
      "vppTokenId": "Guid"
    }
  ]
}
```
