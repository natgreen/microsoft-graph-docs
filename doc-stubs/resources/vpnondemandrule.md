---
title: "vpnOnDemandRule resource type"
description: "VPN On-Demand Rule definition."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# vpnOnDemandRule resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

VPN On-Demand Rule definition.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|vpnOnDemandRuleConnectionAction|Action. Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|dnsSearchDomains|String collection|DNS Search Domains.|
|domainAction|vpnOnDemandRuleConnectionDomainAction|Domain Action (Only applicable when Action is evaluate connection). Possible values are: `connectIfNeeded`, `neverConnect`.|
|domains|String collection|Domains (Only applicable when Action is evaluate connection).|
|probeRequiredUrl|String|Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).|
|probeUrl|String|A URL to probe. If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.|
|ssids|String collection|Network Service Set Identifiers (SSIDs).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "action": "String",
  "dnsSearchDomains": [
    "String"
  ],
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String",
  "probeUrl": "String",
  "ssids": [
    "String"
  ]
}
```
