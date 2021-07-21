---
title: "Create aggregatedPolicyCompliance"
description: "Create a new aggregatedPolicyCompliance object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create aggregatedPolicyCompliance
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) object.

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
POST /tenantRelationships/managedTenants/aggregatedPolicyCompliances
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) object.

The following table shows the properties that are required when you create the [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/managedtenants-entity.md)|
|compliancePolicyId|String|**TODO: Add Description**|
|compliancePolicyName|String|**TODO: Add Description**|
|compliancePolicyPlatform|String|**TODO: Add Description**|
|compliancePolicyType|String|**TODO: Add Description**|
|lastRefreshedDateTime|DateTimeOffset|**TODO: Add Description**|
|numberOfCompliantDevices|Int64|**TODO: Add Description**|
|numberOfErrorDevices|Int64|**TODO: Add Description**|
|numberOfNonCompliantDevices|Int64|**TODO: Add Description**|
|policyModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|tenantDisplayName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_aggregatedpolicycompliance_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/aggregatedPolicyCompliances
Content-Type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.managedTenants.aggregatedPolicyCompliance",
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
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.aggregatedPolicyCompliance"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

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
```
