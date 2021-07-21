---
title: "chatMessage resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# chatMessage resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List chatMessages](../api/chatmessage-list.md)|[chatMessage](../resources/chatmessage.md) collection|Get a list of the [chatMessage](../resources/chatmessage.md) objects and their properties.|
|[Create chatMessage](../api/chatmessage-create.md)|[chatMessage](../resources/chatmessage.md)|Create a new [chatMessage](../resources/chatmessage.md) object.|
|[Get chatMessage](../api/chatmessage-get.md)|[chatMessage](../resources/chatmessage.md)|Read the properties and relationships of a [chatMessage](../resources/chatmessage.md) object.|
|[Update chatMessage](../api/chatmessage-update.md)|[chatMessage](../resources/chatmessage.md)|Update the properties of a [chatMessage](../resources/chatmessage.md) object.|
|[Delete chatMessage](../api/chatmessage-delete.md)|None|Deletes a [chatMessage](../resources/chatmessage.md) object.|
|[delta](../api/chatmessage-delta.md)|[chatMessage](../resources/chatmessage.md) collection|**TODO: Add Description**|
|[List hostedContents](../api/chatmessage-list-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection|Get the chatMessageHostedContent resources from the hostedContents navigation property.|
|[Create chatMessageHostedContent](../api/chatmessage-post-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Create a new chatMessageHostedContent object.|
|[List replies](../api/chatmessage-list-replies.md)|[chatMessage](../resources/chatmessage.md) collection|Get the chatMessage resources from the replies navigation property.|
|[Create chatMessage](../api/chatmessage-post-replies.md)|[chatMessage](../resources/chatmessage.md)|Create a new chatMessage object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attachments|[chatMessageAttachment](../resources/chatmessageattachment.md) collection|**TODO: Add Description**|
|body|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|channelIdentity|[channelIdentity](../resources/channelidentity.md)|**TODO: Add Description**|
|chatId|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|
|etag|String|**TODO: Add Description**|
|eventDetail|[eventMessageDetail](../resources/eventmessagedetail.md)|**TODO: Add Description**|
|from|[chatMessageFromIdentitySet](../resources/chatmessagefromidentityset.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|importance|chatMessageImportance|**TODO: Add Description**. Possible values are: `normal`, `high`, `urgent`.|
|lastEditedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|locale|String|**TODO: Add Description**|
|mentions|[chatMessageMention](../resources/chatmessagemention.md) collection|**TODO: Add Description**|
|messageType|chatMessageType|**TODO: Add Description**. Possible values are: `message`, `chatEvent`, `typing`, `unknownFutureValue`, `systemEventMessage`.|
|policyViolation|[chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md)|**TODO: Add Description**|
|reactions|[chatMessageReaction](../resources/chatmessagereaction.md) collection|**TODO: Add Description**|
|replyToId|String|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|summary|String|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|hostedContents|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection|**TODO: Add Description**|
|replies|[chatMessage](../resources/chatmessage.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessage",
  "id": "String (identifier)",
  "attachments": [
    {
      "@odata.type": "microsoft.graph.chatMessageAttachment"
    }
  ],
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "channelIdentity": {
    "@odata.type": "microsoft.graph.channelIdentity"
  },
  "chatId": "String",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "etag": "String",
  "eventDetail": {
    "@odata.type": "microsoft.graph.eventMessageDetail"
  },
  "from": {
    "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
  },
  "importance": "String",
  "lastEditedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "mentions": [
    {
      "@odata.type": "microsoft.graph.chatMessageMention"
    }
  ],
  "messageType": "String",
  "policyViolation": {
    "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
  },
  "reactions": [
    {
      "@odata.type": "microsoft.graph.chatMessageReaction"
    }
  ],
  "replyToId": "String",
  "subject": "String",
  "summary": "String",
  "webUrl": "String"
}
```
