---
title: "protectSite resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# protectSite resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [labelActionBase](../resources/labelactionbase.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessType|siteAccessType|**TODO: Add Description**. Possible values are: `block`, `full`, `limited`.|
|conditionalAccessProtectionLevelId|String|**TODO: Add Description**|
|name|String|**TODO: Add Description** Inherited from [labelActionBase](../resources/labelactionbase.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.protectSite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.protectSite",
  "name": "String",
  "accessType": "String",
  "conditionalAccessProtectionLevelId": "String"
}
```
