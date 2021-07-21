---
title: "Create managedDeviceComplianceTrend"
description: "Create a new managedDeviceComplianceTrend object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managedDeviceComplianceTrend
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new managedDeviceComplianceTrend object.

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
POST /tenantRelationships/managedTenants/managedDeviceComplianceTrends
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object.

The following table shows the properties that are required when you create the [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/managedtenants-entity.md)|
|compliantDeviceCount|Int32|**TODO: Add Description**|
|configManagerDeviceCount|Int32|**TODO: Add Description**|
|countDateTime|String|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|inGracePeriodDeviceCount|Int32|**TODO: Add Description**|
|noncompliantDeviceCount|Int32|**TODO: Add Description**|
|tenantDisplayName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|unknownDeviceCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_manageddevicecompliancetrend_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceComplianceTrends
Content-Type: application/json
Content-length: 407

{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "compliantDeviceCount": "Integer",
  "configManagerDeviceCount": "Integer",
  "countDateTime": "String",
  "errorDeviceCount": "Integer",
  "inGracePeriodDeviceCount": "Integer",
  "noncompliantDeviceCount": "Integer",
  "tenantDisplayName": "String",
  "tenantId": "String",
  "unknownDeviceCount": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "179e4f4a-4f4a-179e-4a4f-9e174a4f9e17",
  "compliantDeviceCount": "Integer",
  "configManagerDeviceCount": "Integer",
  "countDateTime": "String",
  "errorDeviceCount": "Integer",
  "inGracePeriodDeviceCount": "Integer",
  "noncompliantDeviceCount": "Integer",
  "tenantDisplayName": "String",
  "tenantId": "String",
  "unknownDeviceCount": "Integer"
}
```
