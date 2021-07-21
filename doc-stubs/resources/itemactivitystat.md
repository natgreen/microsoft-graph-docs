---
title: "itemActivityStat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# itemActivityStat resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List itemActivityStats](../api/itemactivitystat-list.md)|[itemActivityStat](../resources/itemactivitystat.md) collection|Get a list of the [itemActivityStat](../resources/itemactivitystat.md) objects and their properties.|
|[Create itemActivityStat](../api/itemactivitystat-create.md)|[itemActivityStat](../resources/itemactivitystat.md)|Create a new [itemActivityStat](../resources/itemactivitystat.md) object.|
|[Get itemActivityStat](../api/itemactivitystat-get.md)|[itemActivityStat](../resources/itemactivitystat.md)|Read the properties and relationships of an [itemActivityStat](../resources/itemactivitystat.md) object.|
|[Update itemActivityStat](../api/itemactivitystat-update.md)|[itemActivityStat](../resources/itemactivitystat.md)|Update the properties of an [itemActivityStat](../resources/itemactivitystat.md) object.|
|[Delete itemActivityStat](../api/itemactivitystat-delete.md)|None|Deletes an [itemActivityStat](../resources/itemactivitystat.md) object.|
|[List activities](../api/itemactivitystat-list-activities.md)|[itemActivity](../resources/itemactivity.md) collection|Get the itemActivity resources from the activities navigation property.|
|[Add itemActivity](../api/itemactivitystat-post-activities.md)|[itemActivity](../resources/itemactivity.md)|Add activities by posting to the activities collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|access|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|create|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|delete|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|edit|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|incompleteData|[incompleteData](../resources/incompletedata.md)|**TODO: Add Description**|
|isTrending|Boolean|**TODO: Add Description**|
|move|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[itemActivity](../resources/itemactivity.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemActivityStat",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemActivityStat",
  "id": "String (identifier)",
  "access": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "create": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "delete": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "edit": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "endDateTime": "String (timestamp)",
  "incompleteData": {
    "@odata.type": "microsoft.graph.incompleteData"
  },
  "isTrending": "Boolean",
  "move": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "startDateTime": "String (timestamp)"
}
```
