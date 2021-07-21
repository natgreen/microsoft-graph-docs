---
title: "Update userAnalytics"
description: "Update the properties of a userAnalytics object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userAnalytics
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [userAnalytics](../resources/useranalytics.md) object.

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
PATCH /me/analytics
PATCH /users/{usersId}/analytics
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userAnalytics](../resources/useranalytics.md) object.

The following table shows the properties that are required when you update the [userAnalytics](../resources/useranalytics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settings|[settings](../resources/settings.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [userAnalytics](../resources/useranalytics.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_useranalytics"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/analytics
Content-Type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.userAnalytics",
  "settings": {
    "@odata.type": "microsoft.graph.settings"
  }
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
  "@odata.type": "#microsoft.graph.userAnalytics",
  "id": "46c2d05e-d05e-46c2-5ed0-c2465ed0c246",
  "settings": {
    "@odata.type": "microsoft.graph.settings"
  }
}
```
