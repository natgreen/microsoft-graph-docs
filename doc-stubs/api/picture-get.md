---
title: "Get picture"
description: "Read the properties and relationships of a picture object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get picture
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [picture](../resources/picture.md) object.

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
GET /financials/companies/{companyId}/picture/{pictureId}
GET /financials/companies/{companyId}/items/{itemId}/picture/{pictureId}
GET /financials/companies/{companyId}/employees/{employeeId}/picture/{pictureId}
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/vendor/picture/{pictureId}
GET /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments/{customerPaymentId}/customer/picture/{pictureId}
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

If successful, this method returns a `200 OK` response code and a [picture](../resources/picture.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_picture"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/picture/{pictureId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.picture"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.picture",
    "id": "8c785410-5410-8c78-1054-788c1054788c",
    "content": "Stream",
    "contentType": "String",
    "height": "Integer",
    "width": "Integer"
  }
}
```
