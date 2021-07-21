---
title: "Add entity"
description: "Add resource by posting to the resource collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add entity
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add resource by posting to the resource collection.

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
POST /users/{usersId}/insights/shared/{sharedInsightId}/resource/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [entity](../resources/entity.md) object.

The following table shows the properties that are required when you create the [entity](../resources/entity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and an [entity](../resources/entity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_entity_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/insights/shared/{sharedInsightId}/resource/$ref
Content-Type: application/json
Content-length: 48

{
  "@odata.type": "#microsoft.graph.entity"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.entity",
  "id": "6bde260e-260e-6bde-0e26-de6b0e26de6b"
}
```
