---
title: "Create filterOperatorSchema"
description: "Create a new filterOperatorSchema object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create filterOperatorSchema
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [filterOperatorSchema](../resources/filteroperatorschema.md) object.

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
POST /filterOperators
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [filterOperatorSchema](../resources/filteroperatorschema.md) object.

The following table shows the properties that are required when you create the [filterOperatorSchema](../resources/filteroperatorschema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|arity|scopeOperatorType|**TODO: Add Description**. Possible values are: `Binary`, `Unary`.|
|multivaluedComparisonType|scopeOperatorMultiValuedComparisonType|**TODO: Add Description**. Possible values are: `All`, `Any`.|
|supportedAttributeTypes|attributeType collection|**TODO: Add Description**. Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`, `DateTime`.|



## Response

If successful, this method returns a `201 Created` response code and a [filterOperatorSchema](../resources/filteroperatorschema.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_filteroperatorschema_from_filteroperators"
}
-->
``` http
POST https://graph.microsoft.com/beta/filterOperators
Content-Type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.filterOperatorSchema",
  "arity": "String",
  "multivaluedComparisonType": "String",
  "supportedAttributeTypes": [
    "String"
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.filterOperatorSchema",
  "id": "b22e5ae2-5ae2-b22e-e25a-2eb2e25a2eb2",
  "arity": "String",
  "multivaluedComparisonType": "String",
  "supportedAttributeTypes": [
    "String"
  ]
}
```
