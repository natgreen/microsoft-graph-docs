---
title: "encryptContent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# encryptContent resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**
This is an abstract type.


Inherits from [labelActionBase](../resources/labelactionbase.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|encryptWith|encryptWith|**TODO: Add Description**. Possible values are: `template`, `userDefinedRights`.|
|name|String|**TODO: Add Description** Inherited from [labelActionBase](../resources/labelactionbase.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptContent",
  "name": "String",
  "encryptWith": "String"
}
```
