---
title: "noncustodialDataSource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# noncustodialDataSource resource type

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List noncustodialDataSources](../api/ediscovery-noncustodialdatasource-list.md)|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) collection|Get a list of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) objects and their properties.|
|[Create noncustodialDataSource](../api/ediscovery-noncustodialdatasource-create.md)|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|Create a new [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.|
|[Get noncustodialDataSource](../api/ediscovery-noncustodialdatasource-get.md)|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|Read the properties and relationships of a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.|
|[Update noncustodialDataSource](../api/ediscovery-noncustodialdatasource-update.md)|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|Update the properties of a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.|
|[Delete noncustodialDataSource](../api/ediscovery-noncustodialdatasource-delete.md)|None|Deletes a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.|
|[release](../api/ediscovery-noncustodialdatasource-release.md)|None|**TODO: Add Description**|
|[updateIndex](../api/ediscovery-noncustodialdatasource-updateindex.md)|None|**TODO: Add Description**|
|[List dataSource](../api/ediscovery-noncustodialdatasource-list-datasource.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection|Get the dataSource resources from the dataSource navigation property.|
|[Create dataSource](../api/ediscovery-noncustodialdatasource-post-datasource.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Create a new dataSource object.|
|[List caseIndexOperation](../api/ediscovery-noncustodialdatasource-list-lastindexoperation.md)|[microsoft.graph.ediscovery.caseIndexOperation](../resources/ediscovery-caseindexoperation.md) collection|Get the caseIndexOperation resources from the lastIndexOperation navigation property.|
|[Add caseIndexOperation](../api/ediscovery-noncustodialdatasource-post-lastindexoperation.md)|[microsoft.graph.ediscovery.caseIndexOperation](../resources/ediscovery-caseindexoperation.md)|Add lastIndexOperation by posting to the lastIndexOperation collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applyHoldToSource|Boolean|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|displayName|String|**TODO: Add Description** Inherited from [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/ediscovery-entity.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|releasedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|status|dataSourceContainerStatus|**TODO: Add Description** Inherited from [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md). Possible values are: `Active`, `Released`, `UnknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|dataSource|[dataSource](../resources/ediscovery-datasource.md)|**TODO: Add Description**|
|lastIndexOperation|[caseIndexOperation](../resources/ediscovery-caseindexoperation.md)|**TODO: Add Description** Inherited from [dataSourceContainer](../resources/datasourcecontainer.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource",
  "baseType": "microsoft.graph.ediscovery.dataSourceContainer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.noncustodialDataSource",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "status": "String",
  "applyHoldToSource": "Boolean"
}
```
