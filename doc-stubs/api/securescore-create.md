---
title: "Create secureScore"
description: "Create a new secureScore object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create secureScore
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [secureScore](../resources/securescore.md) object.

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
POST /security/secureScores
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [secureScore](../resources/securescore.md) object.

The following table shows the properties that are required when you create the [secureScore](../resources/securescore.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activeUserCount|Int32|**TODO: Add Description**|
|averageComparativeScores|[averageComparativeScore](../resources/averagecomparativescore.md) collection|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|controlScores|[controlScore](../resources/controlscore.md) collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|currentScore|Double|**TODO: Add Description**|
|enabledServices|String collection|**TODO: Add Description**|
|licensedUserCount|Int32|**TODO: Add Description**|
|maxScore|Double|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [secureScore](../resources/securescore.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_securescore_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/secureScores
Content-Type: application/json
Content-length: 557

{
  "@odata.type": "#microsoft.graph.secureScore",
  "activeUserCount": "Integer",
  "averageComparativeScores": [
    {
      "@odata.type": "microsoft.graph.averageComparativeScore"
    }
  ],
  "azureTenantId": "String",
  "controlScores": [
    {
      "@odata.type": "microsoft.graph.controlScore"
    }
  ],
  "currentScore": "Double",
  "enabledServices": [
    "String"
  ],
  "licensedUserCount": "Integer",
  "maxScore": "Double",
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
  "@odata.type": "microsoft.graph.secureScore"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.secureScore",
  "id": "140e9815-9815-140e-1598-0e1415980e14",
  "activeUserCount": "Integer",
  "averageComparativeScores": [
    {
      "@odata.type": "microsoft.graph.averageComparativeScore"
    }
  ],
  "azureTenantId": "String",
  "controlScores": [
    {
      "@odata.type": "microsoft.graph.controlScore"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "currentScore": "Double",
  "enabledServices": [
    "String"
  ],
  "licensedUserCount": "Integer",
  "maxScore": "Double",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```
