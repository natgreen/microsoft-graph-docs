---
title: "sharedPCAccountManagerPolicy resource type"
description: "SharedPC Account Manager Policy. Only applies when the account manager is enabled."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# sharedPCAccountManagerPolicy resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

SharedPC Account Manager Policy. Only applies when the account manager is enabled.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountDeletionPolicy|sharedPCAccountDeletionPolicyType|Configures when accounts are deleted. Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.|
|cacheAccountsAboveDiskFreePercentage|Int32|Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts. Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold. Valid values 0 to 100|
|inactiveThresholdDays|Int32|Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days. Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.|
|removeAccountsBelowDiskFreePercentage|Int32|Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space. Accounts that have been inactive the longest will be deleted first. Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold. Valid values 0 to 100|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": "Integer",
  "inactiveThresholdDays": "Integer",
  "removeAccountsBelowDiskFreePercentage": "Integer"
}
```
