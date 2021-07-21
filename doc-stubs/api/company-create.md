---
title: "Create company"
description: "Create a new company object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create company
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [company](../resources/company.md) object.

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
POST /financials/companies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [company](../resources/company.md) object.

The following table shows the properties that are required when you create the [company](../resources/company.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|businessProfileId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|systemVersion|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [company](../resources/company.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_company_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies
Content-Type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.company",
  "businessProfileId": "String",
  "displayName": "String",
  "name": "String",
  "systemVersion": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.company"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.company",
  "id": "45ebf98f-f98f-45eb-8ff9-eb458ff9eb45",
  "businessProfileId": "String",
  "displayName": "String",
  "name": "String",
  "systemVersion": "String"
}
```
