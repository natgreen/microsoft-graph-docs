---
title: "Create secureScoreControlProfile"
description: "Create a new secureScoreControlProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create secureScoreControlProfile
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/secureScoreControlProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.

The following table shows the properties that are required when you create the [secureScoreControlProfile](../resources/securescorecontrolprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|actionType|String|**TODO: Add Description**|
|actionUrl|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|complianceInformation|[complianceInformation](../resources/complianceinformation.md) collection|**TODO: Add Description**|
|controlCategory|String|**TODO: Add Description**|
|controlStateUpdates|[secureScoreControlStateUpdate](../resources/securescorecontrolstateupdate.md) collection|**TODO: Add Description**|
|deprecated|Boolean|**TODO: Add Description**|
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



## Response

If successful, this method returns a `201 Created` response code and a [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_securescorecontrolprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/secureScoreControlProfiles
Content-Type: application/json
Content-length: 810

{
  "@odata.type": "#microsoft.graph.secureScoreControlProfile",
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


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.secureScoreControlProfile",
  "id": "fc3f07f5-07f5-fc3f-f507-3ffcf5073ffc",
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
