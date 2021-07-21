---
title: "enrollmentTroubleshootingEvent resource type"
description: "Event representing an enrollment failure."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# enrollmentTroubleshootingEvent resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Event representing an enrollment failure.


Inherits from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List enrollmentTroubleshootingEvents](../api/enrollmenttroubleshootingevent-list.md)|[enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) collection|Get a list of the [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) objects and their properties.|
|[Create enrollmentTroubleshootingEvent](../api/enrollmenttroubleshootingevent-create.md)|[enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md)|Create a new [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) object.|
|[Get enrollmentTroubleshootingEvent](../api/enrollmenttroubleshootingevent-get.md)|[enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md)|Read the properties and relationships of an [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) object.|
|[Update enrollmentTroubleshootingEvent](../api/enrollmenttroubleshootingevent-update.md)|[enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md)|Update the properties of an [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) object.|
|[Delete enrollmentTroubleshootingEvent](../api/enrollmenttroubleshootingevent-delete.md)|None|Deletes an [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|additionalInformation|[keyValuePair](../resources/keyvaluepair.md) collection|A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).|
|correlationId|String|Id used for tracing the failure in the service. Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).|
|deviceId|String|Azure AD device identifier.|
|enrollmentType|deviceEnrollmentType|Type of the enrollment. Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.|
|eventDateTime|DateTimeOffset|Time when the event occurred . Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).|
|eventName|String|Event Name corresponding to the Troubleshooting Event. It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).|
|failureCategory|deviceEnrollmentFailureReason|Highlevel failure category. Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.|
|failureReason|String|Detailed failure reason.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|managedDeviceIdentifier|String|Device identifier created or collected by Intune.|
|operatingSystem|String|Operating System.|
|osVersion|String|OS Version.|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/devicemanagementtroubleshootingerrordetails.md)|Object containing detailed information about the error and its remediation. Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).|
|userId|String|Identifier for the user that tried to enroll the device.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent",
  "baseType": "microsoft.graph.deviceManagementTroubleshootingEvent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "String (identifier)",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "correlationId": "String",
  "eventDateTime": "String (timestamp)",
  "eventName": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
  },
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String",
  "managedDeviceIdentifier": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String"
}
```
