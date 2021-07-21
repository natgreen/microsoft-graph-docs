---
title: "shared resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# shared resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|owner|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|scope|String|**TODO: Add Description**|
|sharedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|sharedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.shared",
  "owner": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "scope": "String",
  "sharedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "sharedDateTime": "String (timestamp)"
}
```
