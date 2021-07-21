---
title: "addFooter resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# addFooter resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [markContent](../resources/markcontent.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alignment|alignment|**TODO: Add Description**. Possible values are: `left`, `right`, `center`.|
|fontColor|String|**TODO: Add Description** Inherited from [markContent](../resources/markcontent.md).|
|fontSize|Int64|**TODO: Add Description** Inherited from [markContent](../resources/markcontent.md).|
|margin|Int32|**TODO: Add Description**|
|name|String|**TODO: Add Description** Inherited from [labelActionBase](../resources/labelactionbase.md).|
|text|String|**TODO: Add Description** Inherited from [markContent](../resources/markcontent.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.addFooter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.addFooter",
  "name": "String",
  "fontColor": "String",
  "fontSize": "Integer",
  "text": "String",
  "alignment": "String",
  "margin": "Integer"
}
```
