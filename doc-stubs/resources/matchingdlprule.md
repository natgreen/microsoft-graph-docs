---
title: "matchingDlpRule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# matchingDlpRule resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|[dlpActionInfo](../resources/dlpactioninfo.md) collection|**TODO: Add Description**|
|isMostRestrictive|Boolean|**TODO: Add Description**|
|policyId|String|**TODO: Add Description**|
|policyName|String|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|ruleId|String|**TODO: Add Description**|
|ruleMode|ruleMode|**TODO: Add Description**. Possible values are: `audit`, `auditAndNotify`, `enforce`, `pendingDeletion`, `test`.|
|ruleName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.matchingDlpRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.matchingDlpRule",
  "actions": [
    {
      "@odata.type": "microsoft.graph.dlpActionInfo"
    }
  ],
  "isMostRestrictive": "Boolean",
  "policyId": "String",
  "policyName": "String",
  "priority": "Integer",
  "ruleId": "String",
  "ruleMode": "String",
  "ruleName": "String"
}
```
