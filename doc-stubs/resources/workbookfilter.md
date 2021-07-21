---
title: "workbookFilter resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookFilter resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List workbookFilters](../api/workbookfilter-list.md)|[workbookFilter](../resources/workbookfilter.md) collection|Get a list of the [workbookFilter](../resources/workbookfilter.md) objects and their properties.|
|[Create workbookFilter](../api/workbookfilter-create.md)|[workbookFilter](../resources/workbookfilter.md)|Create a new [workbookFilter](../resources/workbookfilter.md) object.|
|[Get workbookFilter](../api/workbookfilter-get.md)|[workbookFilter](../resources/workbookfilter.md)|Read the properties and relationships of a [workbookFilter](../resources/workbookfilter.md) object.|
|[Update workbookFilter](../api/workbookfilter-update.md)|[workbookFilter](../resources/workbookfilter.md)|Update the properties of a [workbookFilter](../resources/workbookfilter.md) object.|
|[Delete workbookFilter](../api/workbookfilter-delete.md)|None|Deletes a [workbookFilter](../resources/workbookfilter.md) object.|
|[apply](../api/workbookfilter-apply.md)|None|**TODO: Add Description**|
|[applyBottomItemsFilter](../api/workbookfilter-applybottomitemsfilter.md)|None|**TODO: Add Description**|
|[applyBottomPercentFilter](../api/workbookfilter-applybottompercentfilter.md)|None|**TODO: Add Description**|
|[applyCellColorFilter](../api/workbookfilter-applycellcolorfilter.md)|None|**TODO: Add Description**|
|[applyCustomFilter](../api/workbookfilter-applycustomfilter.md)|None|**TODO: Add Description**|
|[applyDynamicFilter](../api/workbookfilter-applydynamicfilter.md)|None|**TODO: Add Description**|
|[applyFontColorFilter](../api/workbookfilter-applyfontcolorfilter.md)|None|**TODO: Add Description**|
|[applyIconFilter](../api/workbookfilter-applyiconfilter.md)|None|**TODO: Add Description**|
|[applyTopItemsFilter](../api/workbookfilter-applytopitemsfilter.md)|None|**TODO: Add Description**|
|[applyTopPercentFilter](../api/workbookfilter-applytoppercentfilter.md)|None|**TODO: Add Description**|
|[applyValuesFilter](../api/workbookfilter-applyvaluesfilter.md)|None|**TODO: Add Description**|
|[clear](../api/workbookfilter-clear.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|criteria|[workbookFilterCriteria](../resources/workbookfiltercriteria.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookFilter",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "id": "String (identifier)",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria"
  }
}
```
