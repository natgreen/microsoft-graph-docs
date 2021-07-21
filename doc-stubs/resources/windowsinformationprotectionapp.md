---
title: "windowsInformationProtectionApp resource type"
description: "App for Windows information protection"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsInformationProtectionApp resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

App for Windows information protection
This is an abstract type.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|denied|Boolean|If true, app is denied protection or exemption.|
|description|String|The app's description.|
|displayName|String|App display name.|
|productName|String|The product name.|
|publisherName|String|The publisher name|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "denied": "Boolean",
  "description": "String",
  "displayName": "String",
  "productName": "String",
  "publisherName": "String"
}
```
