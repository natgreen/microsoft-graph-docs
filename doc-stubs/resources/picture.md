---
title: "picture resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# picture resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List pictures](../api/picture-list.md)|[picture](../resources/picture.md) collection|Get a list of the [picture](../resources/picture.md) objects and their properties.|
|[Create picture](../api/picture-create.md)|[picture](../resources/picture.md)|Create a new [picture](../resources/picture.md) object.|
|[Get picture](../api/picture-get.md)|[picture](../resources/picture.md)|Read the properties and relationships of a [picture](../resources/picture.md) object.|
|[Update picture](../api/picture-update.md)|[picture](../resources/picture.md)|Update the properties of a [picture](../resources/picture.md) object.|
|[Delete picture](../api/picture-delete.md)|None|Deletes a [picture](../resources/picture.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream|**TODO: Add Description**|
|contentType|String|**TODO: Add Description**|
|height|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|width|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.picture",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.picture",
  "id": "String (identifier)",
  "content": "Stream",
  "contentType": "String",
  "height": "Integer",
  "width": "Integer"
}
```
