---
title: "windowsDefenderAdvancedThreatProtectionConfiguration resource type"
description: "Windows Defender AdvancedThreatProtection Configuration."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsDefenderAdvancedThreatProtectionConfiguration resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows Defender AdvancedThreatProtection Configuration.


Inherits from [deviceConfiguration](../resources/deviceconfiguration.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List windowsDefenderAdvancedThreatProtectionConfigurations](../api/windowsdefenderadvancedthreatprotectionconfiguration-list.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) collection|Get a list of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) objects and their properties.|
|[Create windowsDefenderAdvancedThreatProtectionConfiguration](../api/windowsdefenderadvancedthreatprotectionconfiguration-create.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md)|Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) object.|
|[Get windowsDefenderAdvancedThreatProtectionConfiguration](../api/windowsdefenderadvancedthreatprotectionconfiguration-get.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md)|Read the properties and relationships of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) object.|
|[Update windowsDefenderAdvancedThreatProtectionConfiguration](../api/windowsdefenderadvancedthreatprotectionconfiguration-update.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md)|Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) object.|
|[Delete windowsDefenderAdvancedThreatProtectionConfiguration](../api/windowsdefenderadvancedthreatprotectionconfiguration-delete.md)|None|Deletes a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) object.|
|[assign](../api/windowsdefenderadvancedthreatprotectionconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|**TODO: Add Description**|
|[assignedAccessMultiModeProfiles](../api/windowsdefenderadvancedthreatprotectionconfiguration-assignedaccessmultimodeprofiles.md)|None|**TODO: Add Description**|
|[windowsPrivacyAccessControls](../api/windowsdefenderadvancedthreatprotectionconfiguration-windowsprivacyaccesscontrols.md)|None|**TODO: Add Description**|
|[getOmaSettingPlainTextValue](../api/windowsdefenderadvancedthreatprotectionconfiguration-getomasettingplaintextvalue.md)|String|**TODO: Add Description**|
|[List assignments](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignment resources from the assignments navigation property.|
|[Create deviceConfigurationAssignment](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Create a new deviceConfigurationAssignment object.|
|[List deviceSettingStateSummaries](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummary resources from the deviceSettingStateSummaries navigation property.|
|[Create settingStateDeviceSummary](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Create a new settingStateDeviceSummary object.|
|[List deviceStatuses](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatus resources from the deviceStatuses navigation property.|
|[Create deviceConfigurationDeviceStatus](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Create a new deviceConfigurationDeviceStatus object.|
|[List deviceConfigurationDeviceOverview](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) collection|Get the deviceConfigurationDeviceOverview resources from the deviceStatusOverview navigation property.|
|[Create deviceConfigurationDeviceOverview](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Create a new deviceConfigurationDeviceOverview object.|
|[List groupAssignments](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignment resources from the groupAssignments navigation property.|
|[Create deviceConfigurationGroupAssignment](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Create a new deviceConfigurationGroupAssignment object.|
|[List userStatuses](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatus resources from the userStatuses navigation property.|
|[Create deviceConfigurationUserStatus](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Create a new deviceConfigurationUserStatus object.|
|[List deviceConfigurationUserOverview](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) collection|Get the deviceConfigurationUserOverview resources from the userStatusOverview navigation property.|
|[Create deviceConfigurationUserOverview](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Create a new deviceConfigurationUserOverview object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|advancedThreatProtectionAutoPopulateOnboardingBlob|Boolean|Auto populate onboarding blob programmatically from Advanced Threat protection service|
|advancedThreatProtectionOffboardingBlob|String|Windows Defender AdvancedThreatProtection Offboarding Blob.|
|advancedThreatProtectionOffboardingFilename|String|Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.|
|advancedThreatProtectionOnboardingBlob|String|Windows Defender AdvancedThreatProtection Onboarding Blob.|
|advancedThreatProtectionOnboardingFilename|String|Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.|
|allowSampleSharing|Boolean|Windows Defender AdvancedThreat   ule|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|enableExpeditedTelemetryReporting|Boolean|Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
  },
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
  },
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": "Boolean",
  "version": "Integer",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": "Boolean",
  "advancedThreatProtectionOffboardingBlob": "String",
  "advancedThreatProtectionOffboardingFilename": "String",
  "advancedThreatProtectionOnboardingBlob": "String",
  "advancedThreatProtectionOnboardingFilename": "String",
  "allowSampleSharing": "Boolean",
  "enableExpeditedTelemetryReporting": "Boolean"
}
```
