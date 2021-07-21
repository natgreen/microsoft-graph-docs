---
title: "List vendor"
description: "Get the vendor resources from the vendor navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List vendor
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the vendor resources from the vendor navigation property.

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
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/vendor
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

If successful, this method returns a `200 OK` response code and a collection of [vendor](../resources/vendor.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_vendor"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/vendor
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.vendor)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vendor",
      "id": "11666435-6435-1166-3564-661135646611",
      "address": {
        "@odata.type": "microsoft.graph.postalAddressType"
      },
      "balance": "Decimal",
      "blocked": "String",
      "currencyCode": "String",
      "currencyId": "Guid",
      "displayName": "String",
      "email": "String",
      "lastModifiedDateTime": "String (timestamp)",
      "number": "String",
      "paymentMethodId": "Guid",
      "paymentTermsId": "Guid",
      "phoneNumber": "String",
      "taxLiable": "Boolean",
      "taxRegistrationNumber": "String",
      "website": "String"
    }
  ]
}
```
