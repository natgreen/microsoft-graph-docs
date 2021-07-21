---
title: "Update governanceRoleDefinition"
description: "Update the properties of a governanceRoleDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update governanceRoleDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [governanceRoleDefinition](../resources/governanceroledefinition.md) object.

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
PATCH /governanceRoleDefinitions/{governanceRoleDefinitionsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [governanceRoleDefinition](../resources/governanceroledefinition.md) object.

The following table shows the properties that are required when you update the [governanceRoleDefinition](../resources/governanceroledefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_governanceroledefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/governanceRoleDefinitions/{governanceRoleDefinitionsId}
Content-Type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.governanceRoleDefinition",
  "displayName": "String",
  "externalId": "String",
  "resourceId": "String",
  "templateId": "String"
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
  "@odata.type": "#microsoft.graph.governanceRoleDefinition",
  "id": "10afc88d-c88d-10af-8dc8-af108dc8af10",
  "displayName": "String",
  "externalId": "String",
  "resourceId": "String",
  "templateId": "String"
}
```
