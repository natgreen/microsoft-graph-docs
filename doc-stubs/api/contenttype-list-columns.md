---
title: "List columns"
description: "Get the columnDefinition resources from the columns navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List columns
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the columnDefinition resources from the columns navigation property.

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
GET /drives/{drivesId}/list/contentTypes/{contentTypeId}/columns
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

If successful, this method returns a `200 OK` response code and a collection of [columnDefinition](../resources/columndefinition.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_columndefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/drives/{drivesId}/list/contentTypes/{contentTypeId}/columns
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.columnDefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.columnDefinition",
      "id": "820fcb44-cb44-820f-44cb-0f8244cb0f82",
      "boolean": {
        "@odata.type": "microsoft.graph.booleanColumn"
      },
      "calculated": {
        "@odata.type": "microsoft.graph.calculatedColumn"
      },
      "choice": {
        "@odata.type": "microsoft.graph.choiceColumn"
      },
      "columnGroup": "String",
      "contentApprovalStatus": {
        "@odata.type": "microsoft.graph.contentApprovalStatusColumn"
      },
      "currency": {
        "@odata.type": "microsoft.graph.currencyColumn"
      },
      "dateTime": {
        "@odata.type": "microsoft.graph.dateTimeColumn"
      },
      "defaultValue": {
        "@odata.type": "microsoft.graph.defaultColumnValue"
      },
      "description": "String",
      "displayName": "String",
      "enforceUniqueValues": "Boolean",
      "geolocation": {
        "@odata.type": "microsoft.graph.geolocationColumn"
      },
      "hidden": "Boolean",
      "hyperlinkOrPicture": {
        "@odata.type": "microsoft.graph.hyperlinkOrPictureColumn"
      },
      "indexed": "Boolean",
      "isDeletable": "Boolean",
      "isReorderable": "Boolean",
      "isSealed": "Boolean",
      "lookup": {
        "@odata.type": "microsoft.graph.lookupColumn"
      },
      "name": "String",
      "number": {
        "@odata.type": "microsoft.graph.numberColumn"
      },
      "personOrGroup": {
        "@odata.type": "microsoft.graph.personOrGroupColumn"
      },
      "propagateChanges": "Boolean",
      "readOnly": "Boolean",
      "required": "Boolean",
      "term": {
        "@odata.type": "microsoft.graph.termColumn"
      },
      "text": {
        "@odata.type": "microsoft.graph.textColumn"
      },
      "thumbnail": {
        "@odata.type": "microsoft.graph.thumbnailColumn"
      },
      "type": "String",
      "validation": {
        "@odata.type": "microsoft.graph.columnValidation"
      }
    }
  ]
}
```
