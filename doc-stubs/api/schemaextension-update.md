---
title: "Update schemaExtension"
description: "Update the properties of a schemaExtension object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update schemaExtension
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [schemaExtension](../resources/schemaextension.md) object.

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
PATCH /schemaExtensions/{schemaExtensionsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.

The following table shows the properties that are required when you update the [schemaExtension](../resources/schemaextension.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description**|
|owner|String|**TODO: Add Description**|
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|targetTypes|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [schemaExtension](../resources/schemaextension.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{schemaExtensionsId}
Content-Type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.schemaExtension",
  "description": "String",
  "owner": "String",
  "properties": [
    {
      "@odata.type": "microsoft.graph.extensionSchemaProperty"
    }
  ],
  "status": "String",
  "targetTypes": [
    "String"
  ]
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
  "@odata.type": "#microsoft.graph.schemaExtension",
  "id": "c020ffab-ffab-c020-abff-20c0abff20c0",
  "description": "String",
  "owner": "String",
  "properties": [
    {
      "@odata.type": "microsoft.graph.extensionSchemaProperty"
    }
  ],
  "status": "String",
  "targetTypes": [
    "String"
  ]
}
```
