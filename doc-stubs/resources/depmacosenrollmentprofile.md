---
title: "depMacOSEnrollmentProfile resource type"
description: "The DepMacOSEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile specific to macOS configuration. This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# depMacOSEnrollmentProfile resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The DepMacOSEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile specific to macOS configuration. This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.


Inherits from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List depMacOSEnrollmentProfiles](../api/depmacosenrollmentprofile-list.md)|[depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) collection|Get a list of the [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) objects and their properties.|
|[Create depMacOSEnrollmentProfile](../api/depmacosenrollmentprofile-create.md)|[depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md)|Create a new [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) object.|
|[Get depMacOSEnrollmentProfile](../api/depmacosenrollmentprofile-get.md)|[depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md)|Read the properties and relationships of a [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) object.|
|[Update depMacOSEnrollmentProfile](../api/depmacosenrollmentprofile-update.md)|[depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md)|Update the properties of a [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) object.|
|[Delete depMacOSEnrollmentProfile](../api/depmacosenrollmentprofile-delete.md)|None|Deletes a [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessibilityScreenDisabled|Boolean|Indicates if Accessibility screen is disabled|
|appleIdDisabled|Boolean|Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|applePayDisabled|Boolean|Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|chooseYourLockScreenDisabled|Boolean|Indicates if iCloud Documents and Desktop screen is disabled|
|configurationEndpointUrl|String|Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/enrollmentprofile.md).|
|configurationWebUrl|Boolean|URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|description|String|Description of the profile Inherited from [enrollmentProfile](../resources/enrollmentprofile.md).|
|deviceNameTemplate|String|Sets a literal or name pattern. Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|diagnosticsDisabled|Boolean|Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|displayName|String|Name of the profile Inherited from [enrollmentProfile](../resources/enrollmentprofile.md).|
|displayToneSetupDisabled|Boolean|Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|enableAuthenticationViaCompanyPortal|Boolean|Indicates to authenticate with Apple Setup Assistant instead of Company Portal. Inherited from [enrollmentProfile](../resources/enrollmentprofile.md).|
|fileVaultDisabled|Boolean|Indicates if file vault is disabled|
|iCloudDiagnosticsDisabled|Boolean|Indicates if iCloud Analytics screen is disabled|
|iCloudStorageDisabled|Boolean|Indicates if iCloud Documents and Desktop screen is disabled|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|isDefault|Boolean|Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|isMandatory|Boolean|Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|locationDisabled|Boolean|Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|passCodeDisabled|Boolean|Indicates if Passcode setup pane is disabled|
|privacyPaneDisabled|Boolean|Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|profileRemovalDisabled|Boolean|Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|registrationDisabled|Boolean|Indicates if registration is disabled|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/enrollmentprofile.md).|
|requiresUserAuthentication|Boolean|Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/enrollmentprofile.md).|
|restoreBlocked|Boolean|Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|screenTimeScreenDisabled|Boolean|Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|siriDisabled|Boolean|Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|supervisedModeEnabled|Boolean|Supervised mode, True to enable, false otherwise. See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information. Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|supportDepartment|String|Support department information Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|supportPhoneNumber|String|Support phone number Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|termsAndConditionsDisabled|Boolean|Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|touchIdDisabled|Boolean|Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md).|
|zoomDisabled|Boolean|Indicates if zoom setup pane is disabled|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depMacOSEnrollmentProfile",
  "baseType": "microsoft.graph.depEnrollmentBaseProfile",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "String (identifier)",
  "configurationEndpointUrl": "String",
  "description": "String",
  "displayName": "String",
  "enableAuthenticationViaCompanyPortal": "Boolean",
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": "Boolean",
  "requiresUserAuthentication": "Boolean",
  "appleIdDisabled": "Boolean",
  "applePayDisabled": "Boolean",
  "configurationWebUrl": "Boolean",
  "deviceNameTemplate": "String",
  "diagnosticsDisabled": "Boolean",
  "displayToneSetupDisabled": "Boolean",
  "isDefault": "Boolean",
  "isMandatory": "Boolean",
  "locationDisabled": "Boolean",
  "privacyPaneDisabled": "Boolean",
  "profileRemovalDisabled": "Boolean",
  "restoreBlocked": "Boolean",
  "screenTimeScreenDisabled": "Boolean",
  "siriDisabled": "Boolean",
  "supervisedModeEnabled": "Boolean",
  "supportDepartment": "String",
  "supportPhoneNumber": "String",
  "termsAndConditionsDisabled": "Boolean",
  "touchIdDisabled": "Boolean",
  "accessibilityScreenDisabled": "Boolean",
  "chooseYourLockScreenDisabled": "Boolean",
  "fileVaultDisabled": "Boolean",
  "iCloudDiagnosticsDisabled": "Boolean",
  "iCloudStorageDisabled": "Boolean",
  "passCodeDisabled": "Boolean",
  "registrationDisabled": "Boolean",
  "zoomDisabled": "Boolean"
}
```
