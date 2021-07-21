---
title: "Create workbookChartLegend"
description: "Create a new workbookChartLegend object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workbookChartLegend
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new workbookChartLegend object.

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
POST /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/legend
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookChartLegend](../resources/workbookchartlegend.md) object.

The following table shows the properties that are required when you create the [workbookChartLegend](../resources/workbookchartlegend.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|overlay|Boolean|**TODO: Add Description**|
|position|String|**TODO: Add Description**|
|visible|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookchartlegend_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/legend
Content-Type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.workbookChartLegend",
  "overlay": "Boolean",
  "position": "String",
  "visible": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.workbookChartLegend",
  "id": "5e5d7620-7620-5e5d-2076-5d5e20765d5e",
  "overlay": "Boolean",
  "position": "String",
  "visible": "Boolean"
}
```
