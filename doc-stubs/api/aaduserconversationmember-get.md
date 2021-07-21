---
title: "Get aadUserConversationMember"
description: "Read the properties and relationships of an aadUserConversationMember object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get aadUserConversationMember
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [aadUserConversationMember](../resources/aaduserconversationmember.md) object.

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
GET /aadUserConversationMember
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

If successful, this method returns a `200 OK` response code and an [aadUserConversationMember](../resources/aaduserconversationmember.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_aaduserconversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/aadUserConversationMember
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "faf74d9b-4d9b-faf7-9b4d-f7fa9b4df7fa",
    "displayName": "String",
    "roles": [
      "String"
    ],
    "visibleHistoryStartDateTime": "String (timestamp)",
    "email": "String",
    "tenantId": "String",
    "userId": "String"
  }
}
```
