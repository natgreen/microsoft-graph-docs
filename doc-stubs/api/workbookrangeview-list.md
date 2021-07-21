---
title: "List workbookRangeViews"
description: "Get a list of the workbookRangeView objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List workbookRangeViews
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [workbookRangeView](../resources/workbookrangeview.md) objects and their properties.

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
GET /workbookRangeView/rows
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

If successful, this method returns a `200 OK` response code and a collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_workbookrangeview"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbookRangeView/rows
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.workbookRangeView)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookRangeView",
      "id": "44f6f894-f894-44f6-94f8-f64494f8f644",
      "cellAddresses": {
        "@odata.type": "microsoft.graph.Json"
      },
      "columnCount": "Integer",
      "formulas": {
        "@odata.type": "microsoft.graph.Json"
      },
      "formulasLocal": {
        "@odata.type": "microsoft.graph.Json"
      },
      "formulasR1C1": {
        "@odata.type": "microsoft.graph.Json"
      },
      "index": "Integer",
      "numberFormat": {
        "@odata.type": "microsoft.graph.Json"
      },
      "rowCount": "Integer",
      "text": {
        "@odata.type": "microsoft.graph.Json"
      },
      "values": {
        "@odata.type": "microsoft.graph.Json"
      },
      "valueTypes": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```
