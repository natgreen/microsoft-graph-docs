---
title: "List applePushNotificationCertificate"
description: "Get the applePushNotificationCertificate resources from the applePushNotificationCertificate navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List applePushNotificationCertificate
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the applePushNotificationCertificate resources from the applePushNotificationCertificate navigation property.

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
GET /deviceManagement/applePushNotificationCertificate
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

If successful, this method returns a `200 OK` response code and a collection of [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_applepushnotificationcertificate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.applePushNotificationCertificate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
      "id": "d680f8c2-f8c2-d680-c2f8-80d6c2f880d6",
      "appleIdentifier": "String",
      "certificate": "String",
      "certificateSerialNumber": "String",
      "certificateUploadFailureReason": "String",
      "certificateUploadStatus": "String",
      "expirationDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "topicIdentifier": "String"
    }
  ]
}
```
