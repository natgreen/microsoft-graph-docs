---
title: "rolePermission resource type"
description: "Contains the set of ResourceActions determining the allowed and not allowed permissions for each role."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# rolePermission resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|String collection|Allowed Actions - Deprecated|
|resourceActions|[resourceAction](../resources/resourceaction.md) collection|Resource Actions each containing a set of allowed and not allowed permissions.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction"
    }
  ]
}
```
