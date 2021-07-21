---
title: "Update termsOfUseContainer"
description: "Update the properties of a termsOfUseContainer object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update termsOfUseContainer
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [termsOfUseContainer](../resources/termsofusecontainer.md) object.

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
PATCH /identityGovernance/termsOfUse
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [termsOfUseContainer](../resources/termsofusecontainer.md) object.

The following table shows the properties that are required when you update the [termsOfUseContainer](../resources/termsofusecontainer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response

If successful, this method returns a `200 OK` response code and an updated [termsOfUseContainer](../resources/termsofusecontainer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_termsofusecontainer"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/termsOfUse
Content-Type: application/json
Content-length: 61

{
  "@odata.type": "#microsoft.graph.termsOfUseContainer"
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
  "@odata.type": "#microsoft.graph.termsOfUseContainer",
  "id": "8df9d14d-d14d-8df9-4dd1-f98d4dd1f98d"
}
```
