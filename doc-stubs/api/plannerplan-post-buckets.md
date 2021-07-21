---
title: "Add plannerBucket"
description: "Add buckets by posting to the buckets collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add plannerBucket
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add buckets by posting to the buckets collection.

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
POST /users/{usersId}/planner/favoritePlans/{plannerPlanId}/buckets/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [plannerBucket](../resources/plannerbucket.md) object.

The following table shows the properties that are required when you create the [plannerBucket](../resources/plannerbucket.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|orderHint|String|**TODO: Add Description**|
|planId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [plannerBucket](../resources/plannerbucket.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/planner/favoritePlans/{plannerPlanId}/buckets/$ref
Content-Type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.plannerBucket",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerBucket",
  "id": "33f5c265-c265-33f5-65c2-f53365c2f533",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}
```
