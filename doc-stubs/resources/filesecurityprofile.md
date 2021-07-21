---
title: "fileSecurityProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# fileSecurityProfile resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List fileSecurityProfiles](../api/filesecurityprofile-list.md)|[fileSecurityProfile](../resources/filesecurityprofile.md) collection|Get a list of the [fileSecurityProfile](../resources/filesecurityprofile.md) objects and their properties.|
|[Create fileSecurityProfile](../api/filesecurityprofile-create.md)|[fileSecurityProfile](../resources/filesecurityprofile.md)|Create a new [fileSecurityProfile](../resources/filesecurityprofile.md) object.|
|[Get fileSecurityProfile](../api/filesecurityprofile-get.md)|[fileSecurityProfile](../resources/filesecurityprofile.md)|Read the properties and relationships of a [fileSecurityProfile](../resources/filesecurityprofile.md) object.|
|[Update fileSecurityProfile](../api/filesecurityprofile-update.md)|[fileSecurityProfile](../resources/filesecurityprofile.md)|Update the properties of a [fileSecurityProfile](../resources/filesecurityprofile.md) object.|
|[Delete fileSecurityProfile](../api/filesecurityprofile-delete.md)|None|Deletes a [fileSecurityProfile](../resources/filesecurityprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityGroupNames|String collection|**TODO: Add Description**|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|certificateThumbprint|String|**TODO: Add Description**|
|extensions|String collection|**TODO: Add Description**|
|fileType|String|**TODO: Add Description**|
|firstSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|hashes|[fileHash](../resources/filehash.md) collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|malwareStates|[malwareState](../resources/malwarestate.md) collection|**TODO: Add Description**|
|names|String collection|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|size|Int64|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|
|vulnerabilityStates|[vulnerabilityState](../resources/vulnerabilitystate.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fileSecurityProfile",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileSecurityProfile",
  "id": "String (identifier)",
  "activityGroupNames": [
    "String"
  ],
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "certificateThumbprint": "String",
  "extensions": [
    "String"
  ],
  "fileType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "hashes": [
    {
      "@odata.type": "microsoft.graph.fileHash"
    }
  ],
  "lastSeenDateTime": "String (timestamp)",
  "malwareStates": [
    {
      "@odata.type": "microsoft.graph.malwareState"
    }
  ],
  "names": [
    "String"
  ],
  "riskScore": "String",
  "size": "Integer",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  },
  "vulnerabilityStates": [
    {
      "@odata.type": "microsoft.graph.vulnerabilityState"
    }
  ]
}
```
