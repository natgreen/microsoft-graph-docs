---
title: "List aggregatedPolicyCompliances"
description: "Get the aggregatedPolicyCompliance resources from the aggregatedPolicyCompliances navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List aggregatedPolicyCompliances
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the aggregatedPolicyCompliance resources from the aggregatedPolicyCompliances navigation property.

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
GET /tenantRelationships/managedTenants/aggregatedPolicyCompliances
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

If successful, this method returns a `200 OK` response code and a collection of [aggregatedPolicyCompliance](../resources/aggregatedpolicycompliance.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_aggregatedpolicycompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/aggregatedPolicyCompliances
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.aggregatedPolicyCompliance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.aggregatedPolicyCompliance",
      "id": "8acdb65d-b65d-8acd-5db6-cd8a5db6cd8a",
      "compliancePolicyId": "String",
      "compliancePolicyName": "String",
      "compliancePolicyPlatform": "String",
      "compliancePolicyType": "String",
      "lastRefreshedDateTime": "String (timestamp)",
      "numberOfCompliantDevices": "Integer",
      "numberOfErrorDevices": "Integer",
      "numberOfNonCompliantDevices": "Integer",
      "policyModifiedDateTime": "String (timestamp)",
      "tenantDisplayName": "String",
      "tenantId": "String"
    }
  ]
}
```
