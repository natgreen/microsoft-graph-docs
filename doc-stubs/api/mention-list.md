---
title: "List mentions"
description: "Get a list of the mention objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List mentions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [mention](../resources/mention.md) objects and their properties.

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
GET /me/mailFolders/{mailFolderId}/messages/{messageId}/mentions
GET /users/{usersId}/mailFolders/{mailFolderId}/messages/{messageId}/mentions
GET /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions
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

If successful, this method returns a `200 OK` response code and a collection of [mention](../resources/mention.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_mention"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/mailFolders/{mailFolderId}/messages/{messageId}/mentions
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.mention)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mention",
      "id": "e7681b5c-1b5c-e768-5c1b-68e75c1b68e7",
      "application": "String",
      "clientReference": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.emailAddress"
      },
      "createdDateTime": "String (timestamp)",
      "deepLink": "String",
      "mentioned": {
        "@odata.type": "microsoft.graph.emailAddress"
      },
      "mentionText": "String",
      "serverCreatedDateTime": "String (timestamp)"
    }
  ]
}
```
