---
title: "paymentMethod resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# paymentMethod resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List paymentMethods](../api/paymentmethod-list.md)|[paymentMethod](../resources/paymentmethod.md) collection|Get a list of the [paymentMethod](../resources/paymentmethod.md) objects and their properties.|
|[Create paymentMethod](../api/paymentmethod-create.md)|[paymentMethod](../resources/paymentmethod.md)|Create a new [paymentMethod](../resources/paymentmethod.md) object.|
|[Get paymentMethod](../api/paymentmethod-get.md)|[paymentMethod](../resources/paymentmethod.md)|Read the properties and relationships of a [paymentMethod](../resources/paymentmethod.md) object.|
|[Update paymentMethod](../api/paymentmethod-update.md)|[paymentMethod](../resources/paymentmethod.md)|Update the properties of a [paymentMethod](../resources/paymentmethod.md) object.|
|[Delete paymentMethod](../api/paymentmethod-delete.md)|None|Deletes a [paymentMethod](../resources/paymentmethod.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.paymentMethod",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.paymentMethod",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```
