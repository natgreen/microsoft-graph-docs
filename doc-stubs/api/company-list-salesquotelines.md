---
title: "List salesQuoteLines"
description: "Get the salesQuoteLine resources from the salesQuoteLines navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List salesQuoteLines
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the salesQuoteLine resources from the salesQuoteLines navigation property.

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
GET /financials/companies/{companyId}/salesQuoteLines
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

If successful, this method returns a `200 OK` response code and a collection of [salesQuoteLine](../resources/salesquoteline.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_salesquoteline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuoteLines
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.salesQuoteLine)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesQuoteLine",
      "id": "a7b9ed0d-ed0d-a7b9-0ded-b9a70dedb9a7",
      "accountId": "Guid",
      "amountExcludingTax": "Decimal",
      "amountIncludingTax": "Decimal",
      "description": "String",
      "discountAmount": "Decimal",
      "discountAppliedBeforeTax": "Boolean",
      "discountPercent": "Decimal",
      "documentId": "Guid",
      "itemId": "Guid",
      "lineType": "String",
      "netAmount": "Decimal",
      "netAmountIncludingTax": "Decimal",
      "netTaxAmount": "Decimal",
      "quantity": "Decimal",
      "sequence": "Integer",
      "taxCode": "String",
      "taxPercent": "Decimal",
      "totalTaxAmount": "Decimal",
      "unitOfMeasureId": "Guid",
      "unitPrice": "Decimal"
    }
  ]
}
```
