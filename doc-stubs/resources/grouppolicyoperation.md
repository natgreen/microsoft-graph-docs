---
title: "groupPolicyOperation resource type"
description: "The entity represents an group policy operation."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyOperation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The entity represents an group policy operation.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List groupPolicyOperations](../api/grouppolicyoperation-list.md)|[groupPolicyOperation](../resources/grouppolicyoperation.md) collection|Get a list of the [groupPolicyOperation](../resources/grouppolicyoperation.md) objects and their properties.|
|[Create groupPolicyOperation](../api/grouppolicyoperation-create.md)|[groupPolicyOperation](../resources/grouppolicyoperation.md)|Create a new [groupPolicyOperation](../resources/grouppolicyoperation.md) object.|
|[Get groupPolicyOperation](../api/grouppolicyoperation-get.md)|[groupPolicyOperation](../resources/grouppolicyoperation.md)|Read the properties and relationships of a [groupPolicyOperation](../resources/grouppolicyoperation.md) object.|
|[Update groupPolicyOperation](../api/grouppolicyoperation-update.md)|[groupPolicyOperation](../resources/grouppolicyoperation.md)|Update the properties of a [groupPolicyOperation](../resources/grouppolicyoperation.md) object.|
|[Delete groupPolicyOperation](../api/grouppolicyoperation-delete.md)|None|Deletes a [groupPolicyOperation](../resources/grouppolicyoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|
|operationStatus|groupPolicyOperationStatus|The group policy operation status. Possible values are: `unknown`, `inProgress`, `success`, `failed`.|
|operationType|groupPolicyOperationType|The type of group policy operation. Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.|
|statusDetails|String|The group policy operation status detail.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "operationStatus": "String",
  "operationType": "String",
  "statusDetails": "String"
}
```
