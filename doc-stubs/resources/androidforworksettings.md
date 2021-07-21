---
title: "androidForWorkSettings resource type"
description: "Settings for Android For Work."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# androidForWorkSettings resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Settings for Android For Work.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List androidForWorkSettings](../api/androidforworksettings-list.md)|[androidForWorkSettings](../resources/androidforworksettings.md) collection|Get a list of the [androidForWorkSettings](../resources/androidforworksettings.md) objects and their properties.|
|[Create androidForWorkSettings](../api/androidforworksettings-create.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Create a new [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[Get androidForWorkSettings](../api/androidforworksettings-get.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Read the properties and relationships of an [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[Update androidForWorkSettings](../api/androidforworksettings-update.md)|[androidForWorkSettings](../resources/androidforworksettings.md)|Update the properties of an [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[Delete androidForWorkSettings](../api/androidforworksettings-delete.md)|None|Deletes an [androidForWorkSettings](../resources/androidforworksettings.md) object.|
|[completeSignup](../api/androidforworksettings-completesignup.md)|None|**TODO: Add Description**|
|[requestSignupUrl](../api/androidforworksettings-requestsignupurl.md)|String|**TODO: Add Description**|
|[syncApps](../api/androidforworksettings-syncapps.md)|None|**TODO: Add Description**|
|[unbind](../api/androidforworksettings-unbind.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bindStatus|androidForWorkBindStatus|Bind status of the tenant with the Google EMM API. Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|deviceOwnerManagementEnabled|Boolean|Indicates if this account is flighting for Android Device Owner Management with CloudDPC.|
|enrollmentTarget|androidForWorkEnrollmentTarget|Indicates which users can enroll devices in Android for Work device management. Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastAppSyncDateTime|DateTimeOffset|Last completion time for app sync|
|lastAppSyncStatus|androidForWorkSyncStatus|Last application sync result. Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|lastModifiedDateTime|DateTimeOffset|Last modification time for Android for Work settings|
|ownerOrganizationName|String|Organization name used when onboarding Android for Work|
|ownerUserPrincipalName|String|Owner UPN that created the enterprise|
|targetGroupIds|String collection|Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "deviceOwnerManagementEnabled": "Boolean",
  "enrollmentTarget": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "ownerOrganizationName": "String",
  "ownerUserPrincipalName": "String",
  "targetGroupIds": [
    "String"
  ]
}
```
