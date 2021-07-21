---
title: "secureScoreControlProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# secureScoreControlProfile resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List secureScoreControlProfiles](../api/securescorecontrolprofile-list.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md) collection|Get a list of the [secureScoreControlProfile](../resources/securescorecontrolprofile.md) objects and their properties.|
|[Create secureScoreControlProfile](../api/securescorecontrolprofile-create.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Create a new [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.|
|[Get secureScoreControlProfile](../api/securescorecontrolprofile-get.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Read the properties and relationships of a [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.|
|[Update secureScoreControlProfile](../api/securescorecontrolprofile-update.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Update the properties of a [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.|
|[Delete secureScoreControlProfile](../api/securescorecontrolprofile-delete.md)|None|Deletes a [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionType|String|**TODO: Add Description**|
|actionUrl|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|complianceInformation|[complianceInformation](../resources/complianceinformation.md) collection|**TODO: Add Description**|
|controlCategory|String|**TODO: Add Description**|
|controlStateUpdates|[secureScoreControlStateUpdate](../resources/securescorecontrolstateupdate.md) collection|**TODO: Add Description**|
|deprecated|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|implementationCost|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|maxScore|Double|**TODO: Add Description**|
|rank|Int32|**TODO: Add Description**|
|remediation|String|**TODO: Add Description**|
|remediationImpact|String|**TODO: Add Description**|
|service|String|**TODO: Add Description**|
|threats|String collection|**TODO: Add Description**|
|tier|String|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|userImpact|String|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.secureScoreControlProfile",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.secureScoreControlProfile",
  "id": "String (identifier)",
  "actionType": "String",
  "actionUrl": "String",
  "azureTenantId": "String",
  "complianceInformation": [
    {
      "@odata.type": "microsoft.graph.complianceInformation"
    }
  ],
  "controlCategory": "String",
  "controlStateUpdates": [
    {
      "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
    }
  ],
  "deprecated": "Boolean",
  "implementationCost": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxScore": "Double",
  "rank": "Integer",
  "remediation": "String",
  "remediationImpact": "String",
  "service": "String",
  "threats": [
    "String"
  ],
  "tier": "String",
  "title": "String",
  "userImpact": "String",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```
