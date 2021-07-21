---
title: "vppTokenLicenseSummary resource type"
description: "License summary of a given app in a token."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# vppTokenLicenseSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

License summary of a given app in a token.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleId|String|The Apple Id associated with the given Apple Volume Purchase Program Token.|
|availableLicenseCount|Int32|The number of VPP licenses available.|
|organizationName|String|The organization associated with the Apple Volume Purchase Program Token.|
|usedLicenseCount|Int32|The number of VPP licenses in use.|
|vppTokenId|String|Identifier of the VPP token.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "appleId": "String",
  "availableLicenseCount": "Integer",
  "organizationName": "String",
  "usedLicenseCount": "Integer",
  "vppTokenId": "String"
}
```
