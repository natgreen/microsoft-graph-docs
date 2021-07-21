---
title: "onPremisesConditionalAccessSettings resource type"
description: "Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onPremisesConditionalAccessSettings resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-list.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) collection|Get a list of the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) objects and their properties.|
|[Create onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-create.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Create a new [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[Get onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Read the properties and relationships of an [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[Update onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-update.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Update the properties of an [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[Delete onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-delete.md)|None|Deletes an [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|enabled|Boolean|Indicates if on premises conditional access is enabled for this organization|
|excludedGroups|Guid collection|User groups that will be exempt by on premises conditional access. All users in these groups will be exempt from the conditional access policy.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|includedGroups|Guid collection|User groups that will be targeted by on premises conditional access. All users in these groups will be required to have mobile device managed and compliant for mail access.|
|overrideDefaultRule|Boolean|Override the default access rule when allowing a device to ensure access is granted.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": "Boolean",
  "excludedGroups": [
    "Guid"
  ],
  "includedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": "Boolean"
}
```
