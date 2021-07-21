---
title: "windowsAutopilotDeploymentProfilePolicySetItem resource type"
description: "A class containing the properties used for windows autopilot deployment profile PolicySetItem."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsAutopilotDeploymentProfilePolicySetItem resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A class containing the properties used for windows autopilot deployment profile PolicySetItem.


Inherits from [policySetItem](../resources/policysetitem.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List windowsAutopilotDeploymentProfilePolicySetItems](../api/windowsautopilotdeploymentprofilepolicysetitem-list.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/windowsautopilotdeploymentprofilepolicysetitem.md) collection|Get a list of the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/windowsautopilotdeploymentprofilepolicysetitem.md) objects and their properties.|
|[Create windowsAutopilotDeploymentProfilePolicySetItem](../api/windowsautopilotdeploymentprofilepolicysetitem-create.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/windowsautopilotdeploymentprofilepolicysetitem.md)|Create a new [windowsAutopilotDeploymentProfilePolicySetItem](../resources/windowsautopilotdeploymentprofilepolicysetitem.md) object.|
|[Get windowsAutopilotDeploymentProfilePolicySetItem](../api/windowsautopilotdeploymentprofilepolicysetitem-get.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/windowsautopilotdeploymentprofilepolicysetitem.md)|Read the properties and relationships of a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/windowsautopilotdeploymentprofilepolicysetitem.md) object.|
|[Update windowsAutopilotDeploymentProfilePolicySetItem](../api/windowsautopilotdeploymentprofilepolicysetitem-update.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/windowsautopilotdeploymentprofilepolicysetitem.md)|Update the properties of a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/windowsautopilotdeploymentprofilepolicysetitem.md) object.|
|[Delete windowsAutopilotDeploymentProfilePolicySetItem](../api/windowsautopilotdeploymentprofilepolicysetitem-delete.md)|None|Deletes a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/windowsautopilotdeploymentprofilepolicysetitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Creation time of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md).|
|displayName|String|DisplayName of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md).|
|errorCode|errorCode|Error code if any occured. Inherited from [policySetItem](../resources/policysetitem.md). Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Tags of the guided deployment Inherited from [policySetItem](../resources/policysetitem.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|itemType|String|policySetType of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md).|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md).|
|payloadId|String|PayloadId of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md).|
|status|policySetStatus|Status of the PolicySetItem. Inherited from [policySetItem](../resources/policysetitem.md). Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
  "baseType": "microsoft.graph.policySetItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ],
  "itemType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "status": "String"
}
```
