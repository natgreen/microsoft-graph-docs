---
title: "extension resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# extension resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**
This is an abstract type.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List extensions](../api/extension-list.md)|[extension](../resources/extension.md) collection|Get a list of the [extension](../resources/extension.md) objects and their properties.|
|[Create extension](../api/extension-create.md)|[extension](../resources/extension.md)|Create a new [extension](../resources/extension.md) object.|
|[Get extension](../api/extension-get.md)|[extension](../resources/extension.md)|Read the properties and relationships of an [extension](../resources/extension.md) object.|
|[Update extension](../api/extension-update.md)|[extension](../resources/extension.md)|Update the properties of an [extension](../resources/extension.md) object.|
|[Delete extension](../api/extension-delete.md)|None|Deletes an [extension](../resources/extension.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.extension",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extension",
  "id": "String (identifier)"
}
```
