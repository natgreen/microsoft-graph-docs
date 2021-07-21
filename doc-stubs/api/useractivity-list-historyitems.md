---
title: "List historyItems"
description: "Get the activityHistoryItem resources from the historyItems navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List historyItems
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the activityHistoryItem resources from the historyItems navigation property.

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
GET /users/{usersId}/activities/{userActivityId}/historyItems
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [activityHistoryItem](../resources/activityhistoryitem.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_activityhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/activities/{userActivityId}/historyItems
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activityHistoryItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.activityHistoryItem",
      "id": "e62fcb5a-cb5a-e62f-5acb-2fe65acb2fe6",
      "activeDurationSeconds": "Integer",
      "createdDateTime": "String (timestamp)",
      "expirationDateTime": "String (timestamp)",
      "lastActiveDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "startedDateTime": "String (timestamp)",
      "status": "String",
      "userTimezone": "String"
    }
  ]
}
```
