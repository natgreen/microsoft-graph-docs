---
title: "updateWindowsDeviceAccountActionParameter resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# updateWindowsDeviceAccountActionParameter resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|calendarSyncEnabled|Boolean|**TODO: Add Description**|
|deviceAccount|[windowsDeviceAccount](../resources/windowsdeviceaccount.md)|**TODO: Add Description**|
|deviceAccountEmail|String|**TODO: Add Description**|
|exchangeServer|String|**TODO: Add Description**|
|passwordRotationEnabled|Boolean|**TODO: Add Description**|
|sessionInitiationProtocalAddress|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "calendarSyncEnabled": "Boolean",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount"
  },
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "passwordRotationEnabled": "Boolean",
  "sessionInitiationProtocalAddress": "String"
}
```
