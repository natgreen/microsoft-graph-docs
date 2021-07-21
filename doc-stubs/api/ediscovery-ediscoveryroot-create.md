---
title: "Create ediscoveryroot"
description: "Create a new ediscoveryroot object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create ediscoveryroot
Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [ediscoveryroot](../resources/ediscovery-ediscoveryroot.md) object.

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
POST ** Collection URI for microsoft.graph.ediscovery.ediscoveryroot not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [ediscoveryroot](../resources/ediscovery-ediscoveryroot.md) object.

The following table shows the properties that are required when you create the [ediscoveryroot](../resources/ediscovery-ediscoveryroot.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/ediscovery-entity.md)|



## Response

If successful, this method returns a `201 Created` response code and an [ediscoveryroot](../resources/ediscovery-ediscoveryroot.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_ediscoveryroot_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.ediscovery.ediscoveryroot not found
Content-Type: application/json
Content-length: 67

{
  "@odata.type": "#microsoft.graph.ediscovery.ediscoveryroot"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.ediscoveryroot"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.ediscovery.ediscoveryroot",
  "id": "f47feb61-eb61-f47f-61eb-7ff461eb7ff4"
}
```
