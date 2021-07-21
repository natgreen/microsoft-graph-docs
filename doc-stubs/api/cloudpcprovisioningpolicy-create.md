---
title: "Create cloudPcProvisioningPolicy"
description: "Create a new cloudPcProvisioningPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create cloudPcProvisioningPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.

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
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.

The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|imageDisplayName|String|**TODO: Add Description**|
|imageId|String|**TODO: Add Description**|
|imageType|cloudPcProvisioningPolicyImageType|**TODO: Add Description**. Possible values are: `gallery`, `custom`.|
|onPremisesConnectionId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_cloudpcprovisioningpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
Content-Type: application/json
Content-length: 245

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "description": "String",
  "displayName": "String",
  "imageDisplayName": "String",
  "imageId": "String",
  "imageType": "String",
  "onPremisesConnectionId": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "944146db-46db-9441-db46-4194db464194",
  "description": "String",
  "displayName": "String",
  "imageDisplayName": "String",
  "imageId": "String",
  "imageType": "String",
  "onPremisesConnectionId": "String"
}
```
