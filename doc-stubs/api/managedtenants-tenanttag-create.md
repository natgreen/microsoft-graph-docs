---
title: "Create tenantTag"
description: "Create a new tenantTag object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create tenantTag
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [tenantTag](../resources/managedtenants-tenanttag.md) object.

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
POST /tenantRelationships/managedTenants/tenantTags
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [tenantTag](../resources/managedtenants-tenanttag.md) object.

The following table shows the properties that are required when you create the [tenantTag](../resources/managedtenants-tenanttag.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/managedtenants-entity.md)|
|createdByUserId|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|lastActionByUserId|String|**TODO: Add Description**|
|lastActionDateTime|DateTimeOffset|**TODO: Add Description**|
|tenants|[microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_tenanttag_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags
Content-Type: application/json
Content-length: 382

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantTag",
  "createdByUserId": "String",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "lastActionByUserId": "String",
  "lastActionDateTime": "String (timestamp)",
  "tenants": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantInfo"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantTag",
  "id": "33abcebd-cebd-33ab-bdce-ab33bdceab33",
  "createdByUserId": "String",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "lastActionByUserId": "String",
  "lastActionDateTime": "String (timestamp)",
  "tenants": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantInfo"
    }
  ]
}
```
