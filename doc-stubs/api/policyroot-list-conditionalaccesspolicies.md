---
title: "List conditionalAccessPolicies"
description: "Get the conditionalAccessPolicy resources from the conditionalAccessPolicies navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List conditionalAccessPolicies
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the conditionalAccessPolicy resources from the conditionalAccessPolicies navigation property.

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
GET /policies/conditionalAccessPolicies
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

If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_conditionalaccesspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/conditionalAccessPolicies
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.conditionalAccessPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.conditionalAccessPolicy",
      "id": "c689e7f3-e7f3-c689-f3e7-89c6f3e789c6",
      "conditions": {
        "@odata.type": "microsoft.graph.conditionalAccessConditionSet"
      },
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "displayName": "String",
      "grantControls": {
        "@odata.type": "microsoft.graph.conditionalAccessGrantControls"
      },
      "modifiedDateTime": "String (timestamp)",
      "sessionControls": {
        "@odata.type": "microsoft.graph.conditionalAccessSessionControls"
      },
      "state": "String"
    }
  ]
}
```
