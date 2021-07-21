---
title: "List subscriptions"
description: "Get the subscription resources from the subscriptions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List subscriptions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the subscription resources from the subscriptions navigation property.

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
GET /workbooks/{workbooksId}/subscriptions
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

If successful, this method returns a `200 OK` response code and a collection of [subscription](../resources/subscription.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_subscription"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/subscriptions
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.subscription)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.subscription",
      "id": "97db9cc1-9cc1-97db-c19c-db97c19cdb97",
      "applicationId": "String",
      "changeType": "String",
      "clientState": "String",
      "creatorId": "String",
      "encryptionCertificate": "String",
      "encryptionCertificateId": "String",
      "expirationDateTime": "String (timestamp)",
      "includeResourceData": "Boolean",
      "latestSupportedTlsVersion": "String",
      "lifecycleNotificationUrl": "String",
      "notificationContentType": "String",
      "notificationQueryOptions": "String",
      "notificationUrl": "String",
      "resource": "String"
    }
  ]
}
```
