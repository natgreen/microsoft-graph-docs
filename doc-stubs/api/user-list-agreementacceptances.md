---
title: "List agreementAcceptances"
description: "Get the agreementAcceptance resources from the agreementAcceptances navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List agreementAcceptances
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the agreementAcceptance resources from the agreementAcceptances navigation property.

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
GET /me/agreementAcceptances
GET /users/{usersId}/agreementAcceptances
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

If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_agreementacceptance"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.agreementAcceptance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.agreementAcceptance",
      "id": "e890bed6-bed6-e890-d6be-90e8d6be90e8",
      "agreementFileId": "String",
      "agreementId": "String",
      "deviceDisplayName": "String",
      "deviceId": "String",
      "deviceOSType": "String",
      "deviceOSVersion": "String",
      "expirationDateTime": "String (timestamp)",
      "recordedDateTime": "String (timestamp)",
      "state": "String",
      "userDisplayName": "String",
      "userEmail": "String",
      "userId": "String",
      "userPrincipalName": "String"
    }
  ]
}
```
