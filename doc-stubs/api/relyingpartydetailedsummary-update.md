---
title: "Update relyingPartyDetailedSummary"
description: "Update the properties of a relyingPartyDetailedSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update relyingPartyDetailedSummary
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object.

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
PATCH /relyingPartyDetailedSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object.

The following table shows the properties that are required when you update the [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|failedSignInCount|Int64|**TODO: Add Description**|
|migrationStatus|migrationStatus|**TODO: Add Description**. Possible values are: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.|
|migrationValidationDetails|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|relyingPartyId|String|**TODO: Add Description**|
|relyingPartyName|String|**TODO: Add Description**|
|replyUrls|String collection|**TODO: Add Description**|
|serviceId|String|**TODO: Add Description**|
|signInSuccessRate|Double|**TODO: Add Description**|
|successfulSignInCount|Int64|**TODO: Add Description**|
|totalSignInCount|Int64|**TODO: Add Description**|
|uniqueUserCount|Int64|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_relyingpartydetailedsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/relyingPartyDetailedSummary
Content-Type: application/json
Content-length: 512

{
  "@odata.type": "#microsoft.graph.relyingPartyDetailedSummary",
  "failedSignInCount": "Integer",
  "migrationStatus": "String",
  "migrationValidationDetails": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "relyingPartyId": "String",
  "relyingPartyName": "String",
  "replyUrls": [
    "String"
  ],
  "serviceId": "String",
  "signInSuccessRate": "Double",
  "successfulSignInCount": "Integer",
  "totalSignInCount": "Integer",
  "uniqueUserCount": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.relyingPartyDetailedSummary",
  "id": "b2565349-5349-b256-4953-56b2495356b2",
  "failedSignInCount": "Integer",
  "migrationStatus": "String",
  "migrationValidationDetails": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "relyingPartyId": "String",
  "relyingPartyName": "String",
  "replyUrls": [
    "String"
  ],
  "serviceId": "String",
  "signInSuccessRate": "Double",
  "successfulSignInCount": "Integer",
  "totalSignInCount": "Integer",
  "uniqueUserCount": "Integer"
}
```
