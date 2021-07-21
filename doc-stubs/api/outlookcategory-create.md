---
title: "Create outlookCategory"
description: "Create a new outlookCategory object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create outlookCategory
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [outlookCategory](../resources/outlookcategory.md) object.

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
POST /me/outlook/masterCategories
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [outlookCategory](../resources/outlookcategory.md) object.

The following table shows the properties that are required when you create the [outlookCategory](../resources/outlookcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|color|categoryColor|**TODO: Add Description**. Possible values are: `none`, `preset0`, `preset1`, `preset2`, `preset3`, `preset4`, `preset5`, `preset6`, `preset7`, `preset8`, `preset9`, `preset10`, `preset11`, `preset12`, `preset13`, `preset14`, `preset15`, `preset16`, `preset17`, `preset18`, `preset19`, `preset20`, `preset21`, `preset22`, `preset23`, `preset24`.|
|displayName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [outlookCategory](../resources/outlookcategory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-Type: application/json
Content-length: 107

{
  "@odata.type": "#microsoft.graph.outlookCategory",
  "color": "String",
  "displayName": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.outlookCategory",
  "id": "2c9f3da9-3da9-2c9f-a93d-9f2ca93d9f2c",
  "color": "String",
  "displayName": "String"
}
```
