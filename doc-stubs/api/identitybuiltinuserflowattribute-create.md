---
title: "Create identityBuiltInUserFlowAttribute"
description: "Create a new identityBuiltInUserFlowAttribute object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create identityBuiltInUserFlowAttribute
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [identityBuiltInUserFlowAttribute](../resources/identitybuiltinuserflowattribute.md) object.

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
POST ** Collection URI for microsoft.graph.identityBuiltInUserFlowAttribute not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [identityBuiltInUserFlowAttribute](../resources/identitybuiltinuserflowattribute.md) object.

The following table shows the properties that are required when you create the [identityBuiltInUserFlowAttribute](../resources/identitybuiltinuserflowattribute.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|dataType|identityUserFlowAttributeDataType|**TODO: Add Description** Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md). Possible values are: `string`, `boolean`, `int64`, `stringCollection`, `dateTime`, `unknownFutureValue`.|
|description|String|**TODO: Add Description** Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|displayName|String|**TODO: Add Description** Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|userFlowAttributeType|identityUserFlowAttributeType|**TODO: Add Description** Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md). Possible values are: `builtIn`, `custom`, `required`, `unknownFutureValue`.|



## Response

If successful, this method returns a `201 Created` response code and an [identityBuiltInUserFlowAttribute](../resources/identitybuiltinuserflowattribute.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_identitybuiltinuserflowattribute_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.identityBuiltInUserFlowAttribute not found
Content-Type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.identityBuiltInUserFlowAttribute",
  "dataType": "String",
  "description": "String",
  "displayName": "String",
  "userFlowAttributeType": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityBuiltInUserFlowAttribute"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.identityBuiltInUserFlowAttribute",
  "id": "d48f9f0c-9f0c-d48f-0c9f-8fd40c9f8fd4",
  "dataType": "String",
  "description": "String",
  "displayName": "String",
  "userFlowAttributeType": "String"
}
```
