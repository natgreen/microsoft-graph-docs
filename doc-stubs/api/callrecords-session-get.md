---
title: "Get session"
description: "Read the properties and relationships of a session object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get session
Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [session](../resources/callrecords-session.md) object.

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
GET /communications/callRecords/{callRecordId}/sessions/{sessionId}
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

If successful, this method returns a `200 OK` response code and a [session](../resources/callrecords-session.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_session"
}
-->
``` http
GET https://graph.microsoft.com/beta/communications/callRecords/{callRecordId}/sessions/{sessionId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.session"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.callRecords.session",
    "id": "152993d3-93d3-1529-d393-2915d3932915",
    "callee": {
      "@odata.type": "microsoft.graph.callRecords.endpoint"
    },
    "caller": {
      "@odata.type": "microsoft.graph.callRecords.endpoint"
    },
    "endDateTime": "String (timestamp)",
    "failureInfo": {
      "@odata.type": "microsoft.graph.callRecords.failureInfo"
    },
    "modalities": [
      "String"
    ],
    "startDateTime": "String (timestamp)"
  }
}
```
