---
title: "Get domainDnsSrvRecord"
description: "Read the properties and relationships of a domainDnsSrvRecord object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get domainDnsSrvRecord
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object.

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
GET /domainDnsSrvRecord
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

If successful, this method returns a `200 OK` response code and a [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_domaindnssrvrecord"
}
-->
``` http
GET https://graph.microsoft.com/beta/domainDnsSrvRecord
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.domainDnsSrvRecord",
    "id": "0d22f132-f132-0d22-32f1-220d32f1220d",
    "isOptional": "Boolean",
    "label": "String",
    "recordType": "String",
    "supportedService": "String",
    "ttl": "Integer",
    "nameTarget": "String",
    "port": "Integer",
    "priority": "Integer",
    "protocol": "String",
    "service": "String",
    "weight": "Integer"
  }
}
```
