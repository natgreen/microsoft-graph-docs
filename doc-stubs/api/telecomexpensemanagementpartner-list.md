---
title: "List telecomExpenseManagementPartners"
description: "Get a list of the telecomExpenseManagementPartner objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List telecomExpenseManagementPartners
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) objects and their properties.

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
GET /deviceManagement/telecomExpenseManagementPartners
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

If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_telecomexpensemanagementpartner"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.telecomExpenseManagementPartner)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
      "id": "a81f2d80-2d80-a81f-802d-1fa8802d1fa8",
      "appAuthorized": "Boolean",
      "displayName": "String",
      "enabled": "Boolean",
      "lastConnectionDateTime": "String (timestamp)",
      "url": "String"
    }
  ]
}
```
