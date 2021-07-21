---
title: "deviceManagementExchangeDeviceClass resource type"
description: "Device Class in Exchange."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementExchangeDeviceClass resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device Class in Exchange.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|name|String|Name of the device class which will be impacted by this rule.|
|type|deviceManagementExchangeAccessRuleType|Type of device which is impacted by this rule e.g. Model, Family. Possible values are: `family`, `model`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```
