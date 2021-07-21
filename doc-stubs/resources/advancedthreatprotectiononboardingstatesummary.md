---
title: "advancedThreatProtectionOnboardingStateSummary resource type"
description: "Windows defender advanced threat protection onboarding state summary across the account."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# advancedThreatProtectionOnboardingStateSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows defender advanced threat protection onboarding state summary across the account.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List advancedThreatProtectionOnboardingStateSummaries](../api/advancedthreatprotectiononboardingstatesummary-list.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) collection|Get a list of the [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) objects and their properties.|
|[Create advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-create.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Create a new [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[Get advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Read the properties and relationships of an [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[Update advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-update.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Update the properties of an [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[Delete advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-delete.md)|None|Deletes an [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[List advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-list-advancedthreatprotectiononboardingdevicesettingstates.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) collection|Get the advancedThreatProtectionOnboardingDeviceSettingState resources from the advancedThreatProtectionOnboardingDeviceSettingStates navigation property.|
|[Create advancedThreatProtectionOnboardingDeviceSettingState](../api/advancedthreatprotectiononboardingstatesummary-post-advancedthreatprotectiononboardingdevicesettingstates.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md)|Create a new advancedThreatProtectionOnboardingDeviceSettingState object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|Number of compliant devices|
|conflictDeviceCount|Int32|Number of conflict devices|
|errorDeviceCount|Int32|Number of error devices|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|nonCompliantDeviceCount|Int32|Number of NonCompliant devices|
|notApplicableDeviceCount|Int32|Number of not applicable devices|
|notAssignedDeviceCount|Int32|Number of not assigned devices|
|remediatedDeviceCount|Int32|Number of remediated devices|
|unknownDeviceCount|Int32|Number of unknown devices|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|advancedThreatProtectionOnboardingDeviceSettingStates|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "String (identifier)",
  "compliantDeviceCount": "Integer",
  "conflictDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "nonCompliantDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "notAssignedDeviceCount": "Integer",
  "remediatedDeviceCount": "Integer",
  "unknownDeviceCount": "Integer"
}
```
