---
title: "Create conversation"
description: "Create a new conversation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create conversation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [conversation](../resources/conversation.md) object.

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
POST /groups/{groupsId}/conversations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [conversation](../resources/conversation.md) object.

The following table shows the properties that are required when you create the [conversation](../resources/conversation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|hasAttachments|Boolean|**TODO: Add Description**|
|lastDeliveredDateTime|DateTimeOffset|**TODO: Add Description**|
|preview|String|**TODO: Add Description**|
|topic|String|**TODO: Add Description**|
|uniqueSenders|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [conversation](../resources/conversation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/conversations
Content-Type: application/json
Content-length: 224

{
  "@odata.type": "#microsoft.graph.conversation",
  "hasAttachments": "Boolean",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "String",
  "topic": "String",
  "uniqueSenders": [
    "String"
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.conversation",
  "id": "157462cb-62cb-1574-cb62-7415cb627415",
  "hasAttachments": "Boolean",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "String",
  "topic": "String",
  "uniqueSenders": [
    "String"
  ]
}
```
