---
title: "Get swapShiftsChangeRequest"
description: "Read the properties and relationships of a swapShiftsChangeRequest object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get swapShiftsChangeRequest
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.

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
GET /teams/{teamsId}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}
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

If successful, this method returns a `200 OK` response code and a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.swapShiftsChangeRequest",
    "id": "7eba75be-75be-7eba-be75-ba7ebe75ba7e",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "assignedTo": "String",
    "managerActionDateTime": "String (timestamp)",
    "managerActionMessage": "String",
    "managerUserId": "String",
    "senderDateTime": "String (timestamp)",
    "senderMessage": "String",
    "senderUserId": "String",
    "state": "String",
    "recipientActionDateTime": "String (timestamp)",
    "recipientActionMessage": "String",
    "recipientUserId": "String",
    "senderShiftId": "String",
    "recipientShiftId": "String"
  }
}
```
