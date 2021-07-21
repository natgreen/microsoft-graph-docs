---
title: "Update serviceHealth"
description: "Update the properties of a serviceHealth object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update serviceHealth
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [serviceHealth](../resources/servicehealth.md) object.

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
PATCH /admin/serviceAnnouncement/healthOverviews/{serviceHealthId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [serviceHealth](../resources/servicehealth.md) object.

The following table shows the properties that are required when you update the [serviceHealth](../resources/servicehealth.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|service|String|**TODO: Add Description**|
|status|serviceHealthStatus|**TODO: Add Description**. Possible values are: `serviceOperational`, `investigating`, `restoringService`, `verifyingService`, `serviceRestored`, `postIncidentReviewPublished`, `serviceDegradation`, `serviceInterruption`, `extendedRecovery`, `falsePositive`, `investigationSuspended`, `resolved`, `mitigatedExternal`, `mitigated`, `resolvedExternal`, `confirmed`, `reported`, `unknownFutureValue`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [serviceHealth](../resources/servicehealth.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_servicehealth"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews/{serviceHealthId}
Content-Type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.serviceHealth",
  "service": "String",
  "status": "String"
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
  "@odata.type": "#microsoft.graph.serviceHealth",
  "id": "e24fdd08-dd08-e24f-08dd-4fe208dd4fe2",
  "service": "String",
  "status": "String"
}
```
