---
title: "admin resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# admin resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get admin](../api/admin-get.md)|[admin](../resources/admin.md)|Read the properties and relationships of an [admin](../resources/admin.md) object.|
|[Update admin](../api/admin-update.md)|[admin](../resources/admin.md)|Update the properties of an [admin](../resources/admin.md) object.|
|[List serviceAnnouncement](../api/admin-list-serviceannouncement.md)|[serviceAnnouncement](../resources/serviceannouncement.md) collection|Get the serviceAnnouncement resources from the serviceAnnouncement navigation property.|
|[Create serviceAnnouncement](../api/admin-post-serviceannouncement.md)|[serviceAnnouncement](../resources/serviceannouncement.md)|Create a new serviceAnnouncement object.|
|[List windows](../api/admin-list-windows.md)|[windows](../resources/windows.md) collection|Get the windows resources from the windows navigation property.|
|[Create windows](../api/admin-post-windows.md)|[windows](../resources/windows.md)|Create a new windows object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|serviceAnnouncement|[serviceAnnouncement](../resources/serviceannouncement.md)|**TODO: Add Description**|
|windows|[windows](../resources/windows.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.admin",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.admin"
}
```
