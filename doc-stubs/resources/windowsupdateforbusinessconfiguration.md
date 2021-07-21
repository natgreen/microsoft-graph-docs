---
title: "windowsUpdateForBusinessConfiguration resource type"
description: "Windows Update for business configuration."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsUpdateForBusinessConfiguration resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows Update for business configuration.


Inherits from [deviceConfiguration](../resources/deviceconfiguration.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List windowsUpdateForBusinessConfigurations](../api/windowsupdateforbusinessconfiguration-list.md)|[windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md) collection|Get a list of the [windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md) objects and their properties.|
|[Create windowsUpdateForBusinessConfiguration](../api/windowsupdateforbusinessconfiguration-create.md)|[windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md)|Create a new [windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md) object.|
|[Get windowsUpdateForBusinessConfiguration](../api/windowsupdateforbusinessconfiguration-get.md)|[windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md)|Read the properties and relationships of a [windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md) object.|
|[Update windowsUpdateForBusinessConfiguration](../api/windowsupdateforbusinessconfiguration-update.md)|[windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md)|Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md) object.|
|[Delete windowsUpdateForBusinessConfiguration](../api/windowsupdateforbusinessconfiguration-delete.md)|None|Deletes a [windowsUpdateForBusinessConfiguration](../resources/windowsupdateforbusinessconfiguration.md) object.|
|[assign](../api/windowsupdateforbusinessconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|**TODO: Add Description**|
|[assignedAccessMultiModeProfiles](../api/windowsupdateforbusinessconfiguration-assignedaccessmultimodeprofiles.md)|None|**TODO: Add Description**|
|[windowsPrivacyAccessControls](../api/windowsupdateforbusinessconfiguration-windowsprivacyaccesscontrols.md)|None|**TODO: Add Description**|
|[getOmaSettingPlainTextValue](../api/windowsupdateforbusinessconfiguration-getomasettingplaintextvalue.md)|String|**TODO: Add Description**|
|[extendFeatureUpdatesPause](../api/windowsupdateforbusinessconfiguration-extendfeatureupdatespause.md)|None|Extend Feature Updates Pause for a Windows Update for Business ring.|
|[extendQualityUpdatesPause](../api/windowsupdateforbusinessconfiguration-extendqualityupdatespause.md)|None|Extend Quality Updates Pause for a Windows Update for Business ring.|
|[List assignments](../api/windowsupdateforbusinessconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignment resources from the assignments navigation property.|
|[Create deviceConfigurationAssignment](../api/windowsupdateforbusinessconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Create a new deviceConfigurationAssignment object.|
|[List deviceSettingStateSummaries](../api/windowsupdateforbusinessconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummary resources from the deviceSettingStateSummaries navigation property.|
|[Create settingStateDeviceSummary](../api/windowsupdateforbusinessconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Create a new settingStateDeviceSummary object.|
|[List deviceStatuses](../api/windowsupdateforbusinessconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatus resources from the deviceStatuses navigation property.|
|[Create deviceConfigurationDeviceStatus](../api/windowsupdateforbusinessconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Create a new deviceConfigurationDeviceStatus object.|
|[List deviceConfigurationDeviceOverview](../api/windowsupdateforbusinessconfiguration-list-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) collection|Get the deviceConfigurationDeviceOverview resources from the deviceStatusOverview navigation property.|
|[Create deviceConfigurationDeviceOverview](../api/windowsupdateforbusinessconfiguration-post-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Create a new deviceConfigurationDeviceOverview object.|
|[List deviceUpdateStates](../api/windowsupdateforbusinessconfiguration-list-deviceupdatestates.md)|[windowsUpdateState](../resources/windowsupdatestate.md) collection|Get the windowsUpdateState resources from the deviceUpdateStates navigation property.|
|[Create windowsUpdateState](../api/windowsupdateforbusinessconfiguration-post-deviceupdatestates.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Create a new windowsUpdateState object.|
|[List groupAssignments](../api/windowsupdateforbusinessconfiguration-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignment resources from the groupAssignments navigation property.|
|[Create deviceConfigurationGroupAssignment](../api/windowsupdateforbusinessconfiguration-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Create a new deviceConfigurationGroupAssignment object.|
|[List userStatuses](../api/windowsupdateforbusinessconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatus resources from the userStatuses navigation property.|
|[Create deviceConfigurationUserStatus](../api/windowsupdateforbusinessconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Create a new deviceConfigurationUserStatus object.|
|[List deviceConfigurationUserOverview](../api/windowsupdateforbusinessconfiguration-list-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) collection|Get the deviceConfigurationUserOverview resources from the userStatusOverview navigation property.|
|[Create deviceConfigurationUserOverview](../api/windowsupdateforbusinessconfiguration-post-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Create a new deviceConfigurationUserOverview object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|automaticUpdateMode|automaticUpdateMode|Automatic update mode. Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.|
|autoRestartNotificationDismissal|autoRestartNotificationDismissalMethod|Specify the method by which the auto-restart required notification is dismissed. Possible values are: `notConfigured`, `automatic`, `user`.|
|businessReadyUpdatesOnly|windowsUpdateType|Determines which branch devices will receive their updates from. Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|deadlineForFeatureUpdatesInDays|Int32|Number of days before feature updates are installed automatically with valid range from 2 to 30 days|
|deadlineForQualityUpdatesInDays|Int32|Number of days before quality updates are installed automatically with valid range from 2 to 30 days|
|deadlineGracePeriodInDays|Int32|Number of days after deadline until restarts occur automatically with valid range from 0 to 7 days|
|deliveryOptimizationMode|windowsDeliveryOptimizationMode|Delivery Optimization Mode. Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|driversExcluded|Boolean|Exclude Windows update Drivers|
|engagedRestartDeadlineInDays|Int32|Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days|
|engagedRestartSnoozeScheduleInDays|Int32|Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days|
|engagedRestartTransitionScheduleInDays|Int32|Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days|
|featureUpdatesDeferralPeriodInDays|Int32|Defer Feature Updates by these many days|
|featureUpdatesPaused|Boolean|Pause Feature Updates|
|featureUpdatesPauseExpiryDateTime|DateTimeOffset|Feature Updates Pause Expiry datetime|
|featureUpdatesPauseStartDate|Date|Feature Updates Pause start date. This property is read-only.|
|featureUpdatesRollbackStartDateTime|DateTimeOffset|Feature Updates Rollback Start datetime|
|featureUpdatesRollbackWindowInDays|Int32|The number of days after a Feature Update for which a rollback is valid|
|featureUpdatesWillBeRolledBack|Boolean|Specifies whether to rollback Feature Updates on the next device check in|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|installationSchedule|[windowsUpdateInstallScheduleType](../resources/windowsupdateinstallscheduletype.md)|Installation schedule|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|microsoftUpdateServiceAllowed|Boolean|Allow Microsoft Update Service|
|postponeRebootUntilAfterDeadline|Boolean|Specifies if the device should wait until deadline for rebooting outside of active hours|
|prereleaseFeatures|prereleaseFeatures|The pre-release features. Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.|
|qualityUpdatesDeferralPeriodInDays|Int32|Defer Quality Updates by these many days|
|qualityUpdatesPaused|Boolean|Pause Quality Updates|
|qualityUpdatesPauseExpiryDateTime|DateTimeOffset|Quality Updates Pause Expiry datetime|
|qualityUpdatesPauseStartDate|Date|Quality Updates Pause start date. This property is read-only.|
|qualityUpdatesRollbackStartDateTime|DateTimeOffset|Quality Updates Rollback Start datetime|
|qualityUpdatesWillBeRolledBack|Boolean|Specifies whether to rollback Quality Updates on the next device check in|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|scheduleImminentRestartWarningInMinutes|Int32|Specify the period for auto-restart imminent warning notifications. Supported values: 15, 30 or 60 (minutes).|
|scheduleRestartWarningInHours|Int32|Specify the period for auto-restart warning reminder notifications. Supported values: 2, 4, 8, 12 or 24 (hours).|
|skipChecksBeforeRestart|Boolean|Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc. |
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|updateNotificationLevel|windowsUpdateNotificationDisplayOption|Specifies what Windows Update notifications users see. Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.|
|updateWeeks|windowsUpdateForBusinessUpdateWeeks|Scheduled the update installation on the weeks of the month. Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.|
|userPauseAccess|enablement|Specifies whether to enable end user’s access to pause software updates. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|userWindowsUpdateScanAccess|enablement|Specifies whether to disable user’s access to scan Windows Update. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceUpdateStates|[windowsUpdateState](../resources/windowsupdatestate.md) collection|Windows update for business configuration device states.|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateForBusinessConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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
  "automaticUpdateMode": "String",
  "autoRestartNotificationDismissal": "String",
  "businessReadyUpdatesOnly": "String",
  "deadlineForFeatureUpdatesInDays": "Integer",
  "deadlineForQualityUpdatesInDays": "Integer",
  "deadlineGracePeriodInDays": "Integer",
  "deliveryOptimizationMode": "String",
  "driversExcluded": "Boolean",
  "engagedRestartDeadlineInDays": "Integer",
  "engagedRestartSnoozeScheduleInDays": "Integer",
  "engagedRestartTransitionScheduleInDays": "Integer",
  "featureUpdatesDeferralPeriodInDays": "Integer",
  "featureUpdatesPaused": "Boolean",
  "featureUpdatesPauseExpiryDateTime": "String (timestamp)",
  "featureUpdatesPauseStartDate": "Date",
  "featureUpdatesRollbackStartDateTime": "String (timestamp)",
  "featureUpdatesRollbackWindowInDays": "Integer",
  "featureUpdatesWillBeRolledBack": "Boolean",
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateInstallScheduleType"
  },
  "microsoftUpdateServiceAllowed": "Boolean",
  "postponeRebootUntilAfterDeadline": "Boolean",
  "prereleaseFeatures": "String",
  "qualityUpdatesDeferralPeriodInDays": "Integer",
  "qualityUpdatesPaused": "Boolean",
  "qualityUpdatesPauseExpiryDateTime": "String (timestamp)",
  "qualityUpdatesPauseStartDate": "Date",
  "qualityUpdatesRollbackStartDateTime": "String (timestamp)",
  "qualityUpdatesWillBeRolledBack": "Boolean",
  "scheduleImminentRestartWarningInMinutes": "Integer",
  "scheduleRestartWarningInHours": "Integer",
  "skipChecksBeforeRestart": "Boolean",
  "updateNotificationLevel": "String",
  "updateWeeks": "String",
  "userPauseAccess": "String",
  "userWindowsUpdateScanAccess": "String"
}
```
