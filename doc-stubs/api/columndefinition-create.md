---
title: "Create columnDefinition"
description: "Create a new columnDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create columnDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [columnDefinition](../resources/columndefinition.md) object.

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
POST /drive/list/columns
POST /sites/{sitesId}/columns
POST /sites/{sitesId}/externalColumns
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [columnDefinition](../resources/columndefinition.md) object.

The following table shows the properties that are required when you create the [columnDefinition](../resources/columndefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|boolean|[booleanColumn](../resources/booleancolumn.md)|**TODO: Add Description**|
|calculated|[calculatedColumn](../resources/calculatedcolumn.md)|**TODO: Add Description**|
|choice|[choiceColumn](../resources/choicecolumn.md)|**TODO: Add Description**|
|columnGroup|String|**TODO: Add Description**|
|contentApprovalStatus|[contentApprovalStatusColumn](../resources/contentapprovalstatuscolumn.md)|**TODO: Add Description**|
|currency|[currencyColumn](../resources/currencycolumn.md)|**TODO: Add Description**|
|dateTime|[dateTimeColumn](../resources/datetimecolumn.md)|**TODO: Add Description**|
|defaultValue|[defaultColumnValue](../resources/defaultcolumnvalue.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|enforceUniqueValues|Boolean|**TODO: Add Description**|
|geolocation|[geolocationColumn](../resources/geolocationcolumn.md)|**TODO: Add Description**|
|hidden|Boolean|**TODO: Add Description**|
|hyperlinkOrPicture|[hyperlinkOrPictureColumn](../resources/hyperlinkorpicturecolumn.md)|**TODO: Add Description**|
|indexed|Boolean|**TODO: Add Description**|
|isDeletable|Boolean|**TODO: Add Description**|
|isReorderable|Boolean|**TODO: Add Description**|
|isSealed|Boolean|**TODO: Add Description**|
|lookup|[lookupColumn](../resources/lookupcolumn.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|number|[numberColumn](../resources/numbercolumn.md)|**TODO: Add Description**|
|personOrGroup|[personOrGroupColumn](../resources/personorgroupcolumn.md)|**TODO: Add Description**|
|propagateChanges|Boolean|**TODO: Add Description**|
|readOnly|Boolean|**TODO: Add Description**|
|required|Boolean|**TODO: Add Description**|
|term|[termColumn](../resources/termcolumn.md)|**TODO: Add Description**|
|text|[textColumn](../resources/textcolumn.md)|**TODO: Add Description**|
|thumbnail|[thumbnailColumn](../resources/thumbnailcolumn.md)|**TODO: Add Description**|
|type|columnTypes|**TODO: Add Description**. Possible values are: `note`, `text`, `choice`, `multichoice`, `number`, `currency`, `dateTime`, `lookup`, `boolean`, `user`, `url`, `calculated`, `location`, `geolocation`, `term`, `multiterm`, `thumbnail`, `approvalStatus`, `unknownFutureValue`.|
|validation|[columnValidation](../resources/columnvalidation.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [columnDefinition](../resources/columndefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_columndefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/drive/list/columns
Content-Type: application/json
Content-length: 1708

{
  "@odata.type": "#microsoft.graph.columnDefinition",
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
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columnDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

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
```
