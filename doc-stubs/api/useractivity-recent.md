---
title: "userActivity: recent"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# userActivity: recent
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

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
GET /me/activities/recent
GET /users/{usersId}/activities/recent
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [userActivity](../resources/useractivity.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "useractivity_recent"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/activities/recent
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userActivity)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userActivity",
      "id": "String (identifier)",
      "activationUrl": "String",
      "activitySourceHost": "String",
      "appActivityId": "String",
      "appDisplayName": "String",
      "contentInfo": {
        "@odata.type": "microsoft.graph.Json"
      },
      "contentUrl": "String",
      "createdDateTime": "String (timestamp)",
      "expirationDateTime": "String (timestamp)",
      "fallbackUrl": "String",
      "lastModifiedDateTime": "String (timestamp)",
      "status": "String",
      "userTimezone": "String",
      "visualElements": {
        "@odata.type": "microsoft.graph.visualInfo"
      }
    }
  ]
}
```
