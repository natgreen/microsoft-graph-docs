---
title: "Create tenantDetailedInformation"
description: "Create a new tenantDetailedInformation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create tenantDetailedInformation
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new tenantDetailedInformation object.

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
POST /tenantRelationships/managedTenants/tenantsDetailedInformation
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) object.

The following table shows the properties that are required when you create the [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/managedtenants-entity.md)|
|city|String|**TODO: Add Description**|
|countryCode|String|**TODO: Add Description**|
|countryName|String|**TODO: Add Description**|
|defaultDomainName|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|industryName|String|**TODO: Add Description**|
|region|String|**TODO: Add Description**|
|segmentName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|verticalName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_tenantdetailedinformation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsDetailedInformation
Content-Type: application/json
Content-length: 355

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantDetailedInformation",
  "city": "String",
  "countryCode": "String",
  "countryName": "String",
  "defaultDomainName": "String",
  "displayName": "String",
  "industryName": "String",
  "region": "String",
  "segmentName": "String",
  "tenantId": "String",
  "verticalName": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantDetailedInformation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantDetailedInformation",
  "id": "1f4736de-36de-1f47-de36-471fde36471f",
  "city": "String",
  "countryCode": "String",
  "countryName": "String",
  "defaultDomainName": "String",
  "displayName": "String",
  "industryName": "String",
  "region": "String",
  "segmentName": "String",
  "tenantId": "String",
  "verticalName": "String"
}
```
