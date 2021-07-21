---
title: "Get unitOfMeasure"
description: "Read the properties and relationships of an unitOfMeasure object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get unitOfMeasure
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [unitOfMeasure](../resources/unitofmeasure.md) object.

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
GET /financials/companies/{companyId}/unitsOfMeasure/{unitOfMeasureId}
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

If successful, this method returns a `200 OK` response code and an [unitOfMeasure](../resources/unitofmeasure.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_unitofmeasure"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/unitsOfMeasure/{unitOfMeasureId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unitOfMeasure"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.unitOfMeasure",
    "id": "ff79457f-457f-ff79-7f45-79ff7f4579ff",
    "code": "String",
    "displayName": "String",
    "internationalStandardCode": "String",
    "lastModifiedDateTime": "String (timestamp)"
  }
}
```
