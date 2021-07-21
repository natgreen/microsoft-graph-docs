---
title: "Create offerShiftRequest"
description: "Create a new offerShiftRequest object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create offerShiftRequest
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new offerShiftRequest object.

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
POST /teams/{teamsId}/schedule/offerShiftRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [offerShiftRequest](../resources/offershiftrequest.md) object.

The following table shows the properties that are required when you create the [offerShiftRequest](../resources/offershiftrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|assignedTo|scheduleChangeRequestActor|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|managerActionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerActionMessage|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerUserId|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderMessage|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderUserId|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|state|scheduleChangeState|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|
|recipientActionDateTime|DateTimeOffset|**TODO: Add Description**|
|recipientActionMessage|String|**TODO: Add Description**|
|recipientUserId|String|**TODO: Add Description**|
|senderShiftId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_offershiftrequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamsId}/schedule/offerShiftRequests
Content-Type: application/json
Content-length: 554

{
  "@odata.type": "#microsoft.graph.offerShiftRequest",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
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
  "senderShiftId": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.offerShiftRequest",
  "id": "21f92ad0-2ad0-21f9-d02a-f921d02af921",
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
  "senderShiftId": "String"
}
```
