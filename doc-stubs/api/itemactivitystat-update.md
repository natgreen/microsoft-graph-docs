---
title: "Update itemActivityStat"
description: "Update the properties of an itemActivityStat object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update itemActivityStat
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [itemActivityStat](../resources/itemactivitystat.md) object.

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
PATCH /workbooks/{workbooksId}/activities/{itemActivityOLDId}/listItem/analytics/allTime
PATCH /workbooks/{workbooksId}/activities/{itemActivityOLDId}/listItem/analytics/lastSevenDays
PATCH /workbooks/{workbooksId}/activities/{itemActivityOLDId}/listItem/analytics/itemActivityStats/{itemActivityStatId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [itemActivityStat](../resources/itemactivitystat.md) object.

The following table shows the properties that are required when you update the [itemActivityStat](../resources/itemactivitystat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|access|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|create|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|delete|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|edit|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|incompleteData|[incompleteData](../resources/incompletedata.md)|**TODO: Add Description**|
|isTrending|Boolean|**TODO: Add Description**|
|move|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [itemActivityStat](../resources/itemactivitystat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_itemactivitystat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/workbooks/{workbooksId}/activities/{itemActivityOLDId}/listItem/analytics/allTime
Content-Type: application/json
Content-length: 616

{
  "@odata.type": "#microsoft.graph.itemActivityStat",
  "access": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "create": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "delete": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "edit": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "endDateTime": "String (timestamp)",
  "incompleteData": {
    "@odata.type": "microsoft.graph.incompleteData"
  },
  "isTrending": "Boolean",
  "move": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "startDateTime": "String (timestamp)"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.itemActivityStat",
  "id": "3d03518d-518d-3d03-8d51-033d8d51033d",
  "access": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "create": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "delete": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "edit": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "endDateTime": "String (timestamp)",
  "incompleteData": {
    "@odata.type": "microsoft.graph.incompleteData"
  },
  "isTrending": "Boolean",
  "move": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "startDateTime": "String (timestamp)"
}
```
