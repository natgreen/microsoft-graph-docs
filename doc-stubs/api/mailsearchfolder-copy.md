---
title: "mailSearchFolder: copy"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# mailSearchFolder: copy
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
POST ** Entity URI for microsoft.graph.mailSearchFolder not found/copy
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
|DestinationId|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [mailFolder](../resources/mailfolder.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "mailsearchfolder_copy"
}
-->
``` http
POST https://graph.microsoft.com/beta** Entity URI for microsoft.graph.mailSearchFolder not found/copy
Content-Type: application/json
Content-length: 33

{
  "DestinationId": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.mailFolder",
    "id": "String (identifier)",
    "childFolderCount": "Integer",
    "displayName": "String",
    "isHidden": "Boolean",
    "parentFolderId": "String",
    "totalItemCount": "Integer",
    "unreadItemCount": "Integer",
    "wellKnownName": "String"
  }
}
```
