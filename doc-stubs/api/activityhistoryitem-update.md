---
title: "Update activityHistoryItem"
description: "Update the properties of an activityHistoryItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update activityHistoryItem
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [activityHistoryItem](../resources/activityhistoryitem.md) object.

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
PATCH /me/activities/{userActivityId}/historyItems/{activityHistoryItemId}
PATCH /users/{usersId}/activities/{userActivityId}/historyItems/{activityHistoryItemId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [activityHistoryItem](../resources/activityhistoryitem.md) object.

The following table shows the properties that are required when you update the [activityHistoryItem](../resources/activityhistoryitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activeDurationSeconds|Int32|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|lastActiveDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|startedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|status|**TODO: Add Description**. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|
|userTimezone|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [activityHistoryItem](../resources/activityhistoryitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_activityhistoryitem"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/activities/{userActivityId}/historyItems/{activityHistoryItemId}
Content-Type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.activityHistoryItem",
  "activeDurationSeconds": "Integer",
  "expirationDateTime": "String (timestamp)",
  "lastActiveDateTime": "String (timestamp)",
  "startedDateTime": "String (timestamp)",
  "status": "String",
  "userTimezone": "String"
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
```
