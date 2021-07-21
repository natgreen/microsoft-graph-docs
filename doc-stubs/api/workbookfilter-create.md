---
title: "Create workbookFilter"
description: "Create a new workbookFilter object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workbookFilter
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [workbookFilter](../resources/workbookfilter.md) object.

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
POST ** Collection URI for microsoft.graph.workbookFilter not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookFilter](../resources/workbookfilter.md) object.

The following table shows the properties that are required when you create the [workbookFilter](../resources/workbookfilter.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|criteria|[workbookFilterCriteria](../resources/workbookfiltercriteria.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookFilter](../resources/workbookfilter.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookfilter_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.workbookFilter not found
Content-Type: application/json
Content-length: 140

{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFilter"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "id": "42df179c-179c-42df-9c17-df429c17df42",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria"
  }
}
```
