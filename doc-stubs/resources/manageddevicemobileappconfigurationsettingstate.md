---
title: "managedDeviceMobileAppConfigurationSettingState resource type"
description: "Managed Device Mobile App Configuration Setting State for a given device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedDeviceMobileAppConfigurationSettingState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Managed Device Mobile App Configuration Setting State for a given device.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|currentValue|String|Current value of setting on device|
|errorCode|Int64|Error code for the setting|
|errorDescription|String|Error description|
|instanceDisplayName|String|Name of setting instance that is being reported.|
|setting|String|The setting that is being reported|
|settingInstanceId|String|SettingInstanceId|
|settingName|String|Localized/user friendly setting name that is being reported|
|sources|[settingSource](../resources/settingsource.md) collection|Contributing policies|
|state|complianceStatus|The compliance state of the setting. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userEmail|String|UserEmail|
|userId|String|UserId|
|userName|String|UserName|
|userPrincipalName|String|UserPrincipalName.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
  "currentValue": "String",
  "errorCode": "Integer",
  "errorDescription": "String",
  "instanceDisplayName": "String",
  "setting": "String",
  "settingInstanceId": "String",
  "settingName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource"
    }
  ],
  "state": "String",
  "userEmail": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```
