---
title: "androidDeviceOwnerScepCertificateProfile resource type"
description: "Android Device Owner SCEP certificate profile"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# androidDeviceOwnerScepCertificateProfile resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Android Device Owner SCEP certificate profile


Inherits from [androidDeviceOwnerCertificateProfileBase](../resources/androiddeviceownercertificateprofilebase.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List androidDeviceOwnerScepCertificateProfiles](../api/androiddeviceownerscepcertificateprofile-list.md)|[androidDeviceOwnerScepCertificateProfile](../resources/androiddeviceownerscepcertificateprofile.md) collection|Get a list of the [androidDeviceOwnerScepCertificateProfile](../resources/androiddeviceownerscepcertificateprofile.md) objects and their properties.|
|[Create androidDeviceOwnerScepCertificateProfile](../api/androiddeviceownerscepcertificateprofile-create.md)|[androidDeviceOwnerScepCertificateProfile](../resources/androiddeviceownerscepcertificateprofile.md)|Create a new [androidDeviceOwnerScepCertificateProfile](../resources/androiddeviceownerscepcertificateprofile.md) object.|
|[Get androidDeviceOwnerScepCertificateProfile](../api/androiddeviceownerscepcertificateprofile-get.md)|[androidDeviceOwnerScepCertificateProfile](../resources/androiddeviceownerscepcertificateprofile.md)|Read the properties and relationships of an [androidDeviceOwnerScepCertificateProfile](../resources/androiddeviceownerscepcertificateprofile.md) object.|
|[Update androidDeviceOwnerScepCertificateProfile](../api/androiddeviceownerscepcertificateprofile-update.md)|[androidDeviceOwnerScepCertificateProfile](../resources/androiddeviceownerscepcertificateprofile.md)|Update the properties of an [androidDeviceOwnerScepCertificateProfile](../resources/androiddeviceownerscepcertificateprofile.md) object.|
|[Delete androidDeviceOwnerScepCertificateProfile](../api/androiddeviceownerscepcertificateprofile-delete.md)|None|Deletes an [androidDeviceOwnerScepCertificateProfile](../resources/androiddeviceownerscepcertificateprofile.md) object.|
|[List assignments](../api/androiddeviceownerscepcertificateprofile-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignment resources from the assignments navigation property.|
|[Create deviceConfigurationAssignment](../api/androiddeviceownerscepcertificateprofile-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Create a new deviceConfigurationAssignment object.|
|[List deviceSettingStateSummaries](../api/androiddeviceownerscepcertificateprofile-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummary resources from the deviceSettingStateSummaries navigation property.|
|[Create settingStateDeviceSummary](../api/androiddeviceownerscepcertificateprofile-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Create a new settingStateDeviceSummary object.|
|[List deviceStatuses](../api/androiddeviceownerscepcertificateprofile-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatus resources from the deviceStatuses navigation property.|
|[Create deviceConfigurationDeviceStatus](../api/androiddeviceownerscepcertificateprofile-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Create a new deviceConfigurationDeviceStatus object.|
|[List deviceConfigurationDeviceOverview](../api/androiddeviceownerscepcertificateprofile-list-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) collection|Get the deviceConfigurationDeviceOverview resources from the deviceStatusOverview navigation property.|
|[Create deviceConfigurationDeviceOverview](../api/androiddeviceownerscepcertificateprofile-post-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Create a new deviceConfigurationDeviceOverview object.|
|[List groupAssignments](../api/androiddeviceownerscepcertificateprofile-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignment resources from the groupAssignments navigation property.|
|[Create deviceConfigurationGroupAssignment](../api/androiddeviceownerscepcertificateprofile-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Create a new deviceConfigurationGroupAssignment object.|
|[List managedDeviceCertificateStates](../api/androiddeviceownerscepcertificateprofile-list-manageddevicecertificatestates.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) collection|Get the managedDeviceCertificateState resources from the managedDeviceCertificateStates navigation property.|
|[Add managedDeviceCertificateState](../api/androiddeviceownerscepcertificateprofile-post-manageddevicecertificatestates.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md)|Add managedDeviceCertificateStates by posting to the managedDeviceCertificateStates collection.|
|[List androidDeviceOwnerTrustedRootCertificate](../api/androiddeviceownerscepcertificateprofile-list-rootcertificate.md)|[androidDeviceOwnerTrustedRootCertificate](../resources/androiddeviceownertrustedrootcertificate.md) collection|Get the androidDeviceOwnerTrustedRootCertificate resources from the rootCertificate navigation property.|
|[Add androidDeviceOwnerTrustedRootCertificate](../api/androiddeviceownerscepcertificateprofile-post-rootcertificate.md)|[androidDeviceOwnerTrustedRootCertificate](../resources/androiddeviceownertrustedrootcertificate.md)|Add rootCertificate by posting to the rootCertificate collection.|
|[List userStatuses](../api/androiddeviceownerscepcertificateprofile-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatus resources from the userStatuses navigation property.|
|[Create deviceConfigurationUserStatus](../api/androiddeviceownerscepcertificateprofile-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Create a new deviceConfigurationUserStatus object.|
|[List deviceConfigurationUserOverview](../api/androiddeviceownerscepcertificateprofile-list-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) collection|Get the deviceConfigurationUserOverview resources from the userStatusOverview navigation property.|
|[Create deviceConfigurationUserOverview](../api/androiddeviceownerscepcertificateprofile-post-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Create a new deviceConfigurationUserOverview object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateStore|certificateStore|Target store certificate. Possible values are: `user`, `machine`.|
|certificateValidityPeriodScale|certificateValidityPeriodScale|Scale for the Certificate Validity Period. Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/androiddeviceownercertificateprofilebase.md). Possible values are: `days`, `months`, `years`.|
|certificateValidityPeriodValue|Int32|Value for the Certificate Validity Period. Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/androiddeviceownercertificateprofilebase.md).|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|customSubjectAlternativeNames|[customSubjectAlternativeName](../resources/customsubjectalternativename.md) collection|Custom Subject Alternative Name Settings. This collection can contain a maximum of 500 elements.|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|extendedKeyUsages|[extendedKeyUsage](../resources/extendedkeyusage.md) collection|Extended Key Usage (EKU) settings. This collection can contain a maximum of 500 elements. Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/androiddeviceownercertificateprofilebase.md).|
|hashAlgorithm|hashAlgorithms|SCEP Hash Algorithm. Possible values are: `sha1`, `sha2`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|keySize|keySize|SCEP Key Size. Possible values are: `size1024`, `size2048`, `size4096`.|
|keyUsage|keyUsages|SCEP Key Usage. Possible values are: `keyEncipherment`, `digitalSignature`.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|renewalThresholdPercentage|Int32|Certificate renewal threshold percentage. Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/androiddeviceownercertificateprofilebase.md).|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md).|
|scepServerUrls|String collection|SCEP Server Url(s)|
|subjectAlternativeNameFormatString|String|Custom String that defines the AAD Attribute.|
|subjectAlternativeNameType|subjectAlternativeNameType|Certificate Subject Alternative Name Type. Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/androiddeviceownercertificateprofilebase.md). Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.|
|subjectNameFormat|subjectNameFormat|Certificate Subject Name Format. Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/androiddeviceownercertificateprofilebase.md). Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|subjectNameFormatString|String|Custom format to use with SubjectNameFormat = Custom. Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US|
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
|managedDeviceCertificateStates|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) collection|Certificate state for devices|
|rootCertificate|[androidDeviceOwnerTrustedRootCertificate](../resources/androiddeviceownertrustedrootcertificate.md)|Trusted Root Certificate. Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/androiddeviceownercertificateprofilebase.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerScepCertificateProfile",
  "baseType": "microsoft.graph.androidDeviceOwnerCertificateProfileBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
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
  "certificateValidityPeriodScale": "String",
  "certificateValidityPeriodValue": "Integer",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage"
    }
  ],
  "renewalThresholdPercentage": "Integer",
  "subjectAlternativeNameType": "String",
  "subjectNameFormat": "String",
  "certificateStore": "String",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName"
    }
  ],
  "hashAlgorithm": "String",
  "keySize": "String",
  "keyUsage": "String",
  "scepServerUrls": [
    "String"
  ],
  "subjectAlternativeNameFormatString": "String",
  "subjectNameFormatString": "String"
}
```
