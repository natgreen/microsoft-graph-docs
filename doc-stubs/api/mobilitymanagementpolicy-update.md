---
title: "Update mobilityManagementPolicy"
description: "Update the properties of a mobilityManagementPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update mobilityManagementPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.

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
PATCH /mobilityManagementPolicies/{mobilityManagementPoliciesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.

The following table shows the properties that are required when you update the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appliesTo|policyScope|**TODO: Add Description**. Possible values are: `none`, `all`, `selected`, `unknownFutureValue`.|
|complianceUrl|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|discoveryUrl|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isValid|Boolean|**TODO: Add Description**|
|termsOfUseUrl|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/mobilityManagementPolicies/{mobilityManagementPoliciesId}
Content-Type: application/json
Content-length: 262

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "appliesTo": "String",
  "complianceUrl": "String",
  "description": "String",
  "discoveryUrl": "String",
  "displayName": "String",
  "isValid": "Boolean",
  "termsOfUseUrl": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "id": "49c3e51d-e51d-49c3-1de5-c3491de5c349",
  "appliesTo": "String",
  "complianceUrl": "String",
  "description": "String",
  "discoveryUrl": "String",
  "displayName": "String",
  "isValid": "Boolean",
  "termsOfUseUrl": "String"
}
```
