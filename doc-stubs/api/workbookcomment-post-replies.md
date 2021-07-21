---
title: "Create workbookCommentReply"
description: "Create a new workbookCommentReply object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workbookCommentReply
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new workbookCommentReply object.

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
POST /workbooks/{workbooksId}/workbook/comments/{workbookCommentId}/replies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookCommentReply](../resources/workbookcommentreply.md) object.

The following table shows the properties that are required when you create the [workbookCommentReply](../resources/workbookcommentreply.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|content|String|**TODO: Add Description**|
|contentType|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookcommentreply_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook/comments/{workbookCommentId}/replies
Content-Type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.workbookCommentReply",
  "content": "String",
  "contentType": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.workbookCommentReply",
  "id": "2f00a29a-a29a-2f00-9aa2-002f9aa2002f",
  "content": "String",
  "contentType": "String"
}
```
