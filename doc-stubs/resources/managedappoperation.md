---
title: "managedAppOperation resource type"
description: "Represents an operation applied against an app registration."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedAppOperation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents an operation applied against an app registration.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedAppOperations](../api/managedappoperation-list.md)|[managedAppOperation](../resources/managedappoperation.md) collection|Get a list of the [managedAppOperation](../resources/managedappoperation.md) objects and their properties.|
|[Create managedAppOperation](../api/managedappoperation-create.md)|[managedAppOperation](../resources/managedappoperation.md)|Create a new [managedAppOperation](../resources/managedappoperation.md) object.|
|[Get managedAppOperation](../api/managedappoperation-get.md)|[managedAppOperation](../resources/managedappoperation.md)|Read the properties and relationships of a [managedAppOperation](../resources/managedappoperation.md) object.|
|[Update managedAppOperation](../api/managedappoperation-update.md)|[managedAppOperation](../resources/managedappoperation.md)|Update the properties of a [managedAppOperation](../resources/managedappoperation.md) object.|
|[Delete managedAppOperation](../api/managedappoperation-delete.md)|None|Deletes a [managedAppOperation](../resources/managedappoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The operation name.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|The last time the app operation was modified.|
|state|String|The current state of the operation|
|version|String|Version of the entity.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```
