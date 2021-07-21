---
title: "importedDeviceIdentity resource type"
description: "The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# importedDeviceIdentity resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List importedDeviceIdentities](../api/importeddeviceidentity-list.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md) collection|Get a list of the [importedDeviceIdentity](../resources/importeddeviceidentity.md) objects and their properties.|
|[Create importedDeviceIdentity](../api/importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md)|Create a new [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.|
|[Get importedDeviceIdentity](../api/importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md)|Read the properties and relationships of an [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.|
|[Update importedDeviceIdentity](../api/importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md)|Update the properties of an [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.|
|[Delete importedDeviceIdentity](../api/importeddeviceidentity-delete.md)|None|Deletes an [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.|
|[importDeviceIdentityList](../api/importeddeviceidentity-importdeviceidentitylist.md)|[importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) collection|**TODO: Add Description**|
|[searchExistingIdentities](../api/importeddeviceidentity-searchexistingidentities.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md) collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Created Date Time of the device|
|description|String|The description of the device|
|enrollmentState|enrollmentState|The state of the device in Intune. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|importedDeviceIdentifier|String|Imported Device Identifier|
|importedDeviceIdentityType|importedDeviceIdentityType|Type of Imported Device Identity. Possible values are: `unknown`, `imei`, `serialNumber`.|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device|
|lastModifiedDateTime|DateTimeOffset|Last Modified DateTime of the description|
|platform|platform|The platform of the Device. Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastContactedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "platform": "String"
}
```
