---
title: "Create privilegedOperationEvent"
description: "Create a new privilegedOperationEvent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create privilegedOperationEvent
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.

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
POST /privilegedOperationEvents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.

The following table shows the properties that are required when you create the [privilegedOperationEvent](../resources/privilegedoperationevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|additionalInformation|String|**TODO: Add Description**|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|referenceKey|String|**TODO: Add Description**|
|referenceSystem|String|**TODO: Add Description**|
|requestorId|String|**TODO: Add Description**|
|requestorName|String|**TODO: Add Description**|
|requestType|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|roleName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userMail|String|**TODO: Add Description**|
|userName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [privilegedOperationEvent](../resources/privilegedoperationevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_privilegedoperationevent_from_privilegedoperationevents"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedOperationEvents
Content-Type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "additionalInformation": "String",
  "creationDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "referenceKey": "String",
  "referenceSystem": "String",
  "requestorId": "String",
  "requestorName": "String",
  "requestType": "String",
  "roleId": "String",
  "roleName": "String",
  "tenantId": "String",
  "userId": "String",
  "userMail": "String",
  "userName": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "id": "b2186014-6014-b218-1460-18b2146018b2",
  "additionalInformation": "String",
  "creationDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "referenceKey": "String",
  "referenceSystem": "String",
  "requestorId": "String",
  "requestorName": "String",
  "requestType": "String",
  "roleId": "String",
  "roleName": "String",
  "tenantId": "String",
  "userId": "String",
  "userMail": "String",
  "userName": "String"
}
```
