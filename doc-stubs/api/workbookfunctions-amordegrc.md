---
title: "workbookFunctions: amorDegrc"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# workbookFunctions: amorDegrc
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

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
POST /workbooks/{workbooksId}/workbook/functions/amorDegrc
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|cost|[Json](../resources/json.md)|**TODO: Add Description**|
|datePurchased|[Json](../resources/json.md)|**TODO: Add Description**|
|firstPeriod|[Json](../resources/json.md)|**TODO: Add Description**|
|salvage|[Json](../resources/json.md)|**TODO: Add Description**|
|period|[Json](../resources/json.md)|**TODO: Add Description**|
|rate|[Json](../resources/json.md)|**TODO: Add Description**|
|basis|[Json](../resources/json.md)|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [workbookFunctionResult](../resources/workbookfunctionresult.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "workbookfunctions_amordegrc"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook/functions/amorDegrc
Content-Type: application/json
Content-length: 459

{
  "cost": {
    "@odata.type": "microsoft.graph.Json"
  },
  "datePurchased": {
    "@odata.type": "microsoft.graph.Json"
  },
  "firstPeriod": {
    "@odata.type": "microsoft.graph.Json"
  },
  "salvage": {
    "@odata.type": "microsoft.graph.Json"
  },
  "period": {
    "@odata.type": "microsoft.graph.Json"
  },
  "rate": {
    "@odata.type": "microsoft.graph.Json"
  },
  "basis": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFunctionResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "id": "String (identifier)",
    "error": "String",
    "value": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```
