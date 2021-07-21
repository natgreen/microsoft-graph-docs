---
title: "windowsKioskDesktopApp resource type"
description: "The base class for a type of apps"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsKioskDesktopApp resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The base class for a type of apps


Inherits from [windowsKioskAppBase](../resources/windowskioskappbase.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appType|windowsKioskAppType|The app type Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Boolean|Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md).|
|desktopApplicationId|String|Define the DesktopApplicationID of the app|
|desktopApplicationLinkPath|String|Define the DesktopApplicationLinkPath of the app|
|name|String|Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md).|
|path|String|Define the path of a desktop app|
|startLayoutTileSize|windowsAppStartLayoutTileSize|The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "appType": "String",
  "autoLaunch": "Boolean",
  "name": "String",
  "startLayoutTileSize": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String",
  "path": "String"
}
```
