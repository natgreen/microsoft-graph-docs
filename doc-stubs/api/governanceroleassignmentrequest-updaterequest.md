---
title: "governanceRoleAssignmentRequest: updateRequest"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# governanceRoleAssignmentRequest: updateRequest
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

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
POST /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/updateRequest
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|decision|String|**TODO: Add Description**|
|assignmentState|String|**TODO: Add Description**|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|**TODO: Add Description**|
|reason|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_updaterequest"
}
-->
``` http
POST https://graph.microsoft.com/beta/governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/updateRequest
Content-Type: application/json
Content-length: 163

{
  "decision": "String",
  "assignmentState": "String",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule"
  },
  "reason": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
    "id": "String (identifier)",
    "assignmentState": "String",
    "linkedEligibleRoleAssignmentId": "String",
    "reason": "String",
    "requestedDateTime": "String (timestamp)",
    "resourceId": "String",
    "roleDefinitionId": "String",
    "schedule": {
      "@odata.type": "microsoft.graph.governanceSchedule"
    },
    "status": {
      "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
    },
    "subjectId": "String",
    "type": "String"
  }
}
```
