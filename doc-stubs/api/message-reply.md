---
title: "message: reply"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# message: reply
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
POST /me/messages/{messageId}/reply
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|Message|[message](../resources/message.md)|**TODO: Add Description**|
|Comment|String|**TODO: Add Description**|



## Response

If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "message_reply"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/messages/{messageId}/reply
Content-Type: application/json
Content-length: 1931

{
  "Message": {
    "@odata.type": "#microsoft.graph.message",
    "id": "String (identifier)",
    "categories": [
      "String"
    ],
    "changeKey": "String",
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "bccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "body": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "bodyPreview": "String",
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "conversationId": "String",
    "conversationIndex": "Binary",
    "flag": {
      "@odata.type": "microsoft.graph.followupFlag"
    },
    "from": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "hasAttachments": "Boolean",
    "importance": "String",
    "inferenceClassification": "String",
    "internetMessageHeaders": [
      {
        "@odata.type": "microsoft.graph.internetMessageHeader"
      }
    ],
    "internetMessageId": "String",
    "isDeliveryReceiptRequested": "Boolean",
    "isDraft": "Boolean",
    "isRead": "Boolean",
    "isReadReceiptRequested": "Boolean",
    "mentionsPreview": {
      "@odata.type": "microsoft.graph.mentionsPreview"
    },
    "parentFolderId": "String",
    "receivedDateTime": "String (timestamp)",
    "replyTo": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "sender": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "sentDateTime": "String (timestamp)",
    "subject": "String",
    "toRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "uniqueBody": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "unsubscribeData": [
      "String"
    ],
    "unsubscribeEnabled": "Boolean",
    "webLink": "String"
  },
  "Comment": "String"
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
HTTP/1.1 204 No Content
```
