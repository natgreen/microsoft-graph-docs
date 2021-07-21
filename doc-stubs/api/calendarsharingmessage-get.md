---
title: "Get calendarSharingMessage"
description: "Read the properties and relationships of a calendarSharingMessage object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get calendarSharingMessage
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [calendarSharingMessage](../resources/calendarsharingmessage.md) object.

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
GET ** Entity URI for microsoft.graph.calendarSharingMessage not found
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

If successful, this method returns a `200 OK` response code and a [calendarSharingMessage](../resources/calendarsharingmessage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_calendarsharingmessage"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.graph.calendarSharingMessage not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarSharingMessage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.calendarSharingMessage",
    "id": "3ea2edc5-edc5-3ea2-c5ed-a23ec5eda23e",
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
    "webLink": "String",
    "canAccept": "Boolean",
    "sharingMessageAction": {
      "@odata.type": "microsoft.graph.calendarSharingMessageAction"
    },
    "sharingMessageActions": [
      {
        "@odata.type": "microsoft.graph.calendarSharingMessageAction"
      }
    ],
    "suggestedCalendarName": "String"
  }
}
```
