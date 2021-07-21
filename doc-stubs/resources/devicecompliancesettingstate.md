---
title: "deviceComplianceSettingState resource type"
description: "Device compliance setting State for a given device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceComplianceSettingState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device compliance setting State for a given device.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceComplianceSettingStates](../api/devicecompliancesettingstate-list.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) collection|Get a list of the [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) objects and their properties.|
|[Create deviceComplianceSettingState](../api/devicecompliancesettingstate-create.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Create a new [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) object.|
|[Get deviceComplianceSettingState](../api/devicecompliancesettingstate-get.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Read the properties and relationships of a [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) object.|
|[Update deviceComplianceSettingState](../api/devicecompliancesettingstate-update.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Update the properties of a [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) object.|
|[Delete deviceComplianceSettingState](../api/devicecompliancesettingstate-delete.md)|None|Deletes a [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires|
|deviceId|String|The Device Id that is being reported|
|deviceModel|String|The device model that is being reported|
|deviceName|String|The Device Name that is being reported|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|platformType|deviceType|Device platform type. Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `chromeOS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.|
|setting|String|The setting class name and property name.|
|settingName|String|The Setting Name that is being reported|
|state|complianceStatus|The compliance state of the setting. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userEmail|String|The User email address that is being reported|
|userId|String|The user Id that is being reported|
|userName|String|The User Name that is being reported|
|userPrincipalName|String|The User PrincipalName that is being reported|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "deviceId": "String",
  "deviceModel": "String",
  "deviceName": "String",
  "platformType": "String",
  "setting": "String",
  "settingName": "String",
  "state": "String",
  "userEmail": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```
