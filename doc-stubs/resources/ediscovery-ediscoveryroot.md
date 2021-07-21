---
title: "ediscoveryroot resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# ediscoveryroot resource type

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/ediscovery-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List ediscoveryroots](../api/ediscovery-ediscoveryroot-list.md)|[microsoft.graph.ediscovery.ediscoveryroot](../resources/ediscovery-ediscoveryroot.md) collection|Get a list of the [ediscoveryroot](../resources/ediscovery-ediscoveryroot.md) objects and their properties.|
|[Create ediscoveryroot](../api/ediscovery-ediscoveryroot-create.md)|[microsoft.graph.ediscovery.ediscoveryroot](../resources/ediscovery-ediscoveryroot.md)|Create a new [ediscoveryroot](../resources/ediscovery-ediscoveryroot.md) object.|
|[Get ediscoveryroot](../api/ediscovery-ediscoveryroot-get.md)|[microsoft.graph.ediscovery.ediscoveryroot](../resources/ediscovery-ediscoveryroot.md)|Read the properties and relationships of an [ediscoveryroot](../resources/ediscovery-ediscoveryroot.md) object.|
|[Update ediscoveryroot](../api/ediscovery-ediscoveryroot-update.md)|[microsoft.graph.ediscovery.ediscoveryroot](../resources/ediscovery-ediscoveryroot.md)|Update the properties of an [ediscoveryroot](../resources/ediscovery-ediscoveryroot.md) object.|
|[Delete ediscoveryroot](../api/ediscovery-ediscoveryroot-delete.md)|None|Deletes an [ediscoveryroot](../resources/ediscovery-ediscoveryroot.md) object.|
|[List cases](../api/ediscovery-ediscoveryroot-list-cases.md)|[microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) collection|Get the case resources from the cases navigation property.|
|[Create case](../api/ediscovery-ediscoveryroot-post-cases.md)|[microsoft.graph.ediscovery.case](../resources/ediscovery-case.md)|Create a new case object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/ediscovery-entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|cases|[microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.ediscoveryroot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.ediscoveryroot",
  "id": "String (identifier)"
}
```
