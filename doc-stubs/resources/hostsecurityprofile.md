---
title: "hostSecurityProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# hostSecurityProfile resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List hostSecurityProfiles](../api/hostsecurityprofile-list.md)|[hostSecurityProfile](../resources/hostsecurityprofile.md) collection|Get a list of the [hostSecurityProfile](../resources/hostsecurityprofile.md) objects and their properties.|
|[Create hostSecurityProfile](../api/hostsecurityprofile-create.md)|[hostSecurityProfile](../resources/hostsecurityprofile.md)|Create a new [hostSecurityProfile](../resources/hostsecurityprofile.md) object.|
|[Get hostSecurityProfile](../api/hostsecurityprofile-get.md)|[hostSecurityProfile](../resources/hostsecurityprofile.md)|Read the properties and relationships of a [hostSecurityProfile](../resources/hostsecurityprofile.md) object.|
|[Update hostSecurityProfile](../api/hostsecurityprofile-update.md)|[hostSecurityProfile](../resources/hostsecurityprofile.md)|Update the properties of a [hostSecurityProfile](../resources/hostsecurityprofile.md) object.|
|[Delete hostSecurityProfile](../api/hostsecurityprofile-delete.md)|None|Deletes a [hostSecurityProfile](../resources/hostsecurityprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|firstSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|fqdn|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|isAzureAdJoined|Boolean|**TODO: Add Description**|
|isAzureAdRegistered|Boolean|**TODO: Add Description**|
|isHybridAzureDomainJoined|Boolean|**TODO: Add Description**|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|logonUsers|[logonUser](../resources/logonuser.md) collection|**TODO: Add Description**|
|netBiosName|String|**TODO: Add Description**|
|networkInterfaces|[networkInterface](../resources/networkinterface.md) collection|**TODO: Add Description**|
|os|String|**TODO: Add Description**|
|osVersion|String|**TODO: Add Description**|
|parentHost|String|**TODO: Add Description**|
|relatedHostIds|String collection|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hostSecurityProfile",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hostSecurityProfile",
  "id": "String (identifier)",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "firstSeenDateTime": "String (timestamp)",
  "fqdn": "String",
  "isAzureAdJoined": "Boolean",
  "isAzureAdRegistered": "Boolean",
  "isHybridAzureDomainJoined": "Boolean",
  "lastSeenDateTime": "String (timestamp)",
  "logonUsers": [
    {
      "@odata.type": "microsoft.graph.logonUser"
    }
  ],
  "netBiosName": "String",
  "networkInterfaces": [
    {
      "@odata.type": "microsoft.graph.networkInterface"
    }
  ],
  "os": "String",
  "osVersion": "String",
  "parentHost": "String",
  "relatedHostIds": [
    "String"
  ],
  "riskScore": "String",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```
