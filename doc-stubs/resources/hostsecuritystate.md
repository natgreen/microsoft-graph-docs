---
title: "hostSecurityState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# hostSecurityState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fqdn|String|**TODO: Add Description**|
|isAzureAdJoined|Boolean|**TODO: Add Description**|
|isAzureAdRegistered|Boolean|**TODO: Add Description**|
|isHybridAzureDomainJoined|Boolean|**TODO: Add Description**|
|netBiosName|String|**TODO: Add Description**|
|os|String|**TODO: Add Description**|
|privateIpAddress|String|**TODO: Add Description**|
|publicIpAddress|String|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hostSecurityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hostSecurityState",
  "fqdn": "String",
  "isAzureAdJoined": "Boolean",
  "isAzureAdRegistered": "Boolean",
  "isHybridAzureDomainJoined": "Boolean",
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}
```
