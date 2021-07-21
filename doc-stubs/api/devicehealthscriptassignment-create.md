---
title: "Create deviceHealthScriptAssignment"
description: "Create a new deviceHealthScriptAssignment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceHealthScriptAssignment
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object.

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
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object.

The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|runRemediationScript|Boolean|Determine whether we want to run detection script only or run both detection script and remediation script|
|runSchedule|[deviceHealthScriptRunSchedule](../resources/devicehealthscriptrunschedule.md)|Script run schedule for the target group|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The Azure Active Directory group we are targeting the script to|



## Response

If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicehealthscriptassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
Content-Type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "runRemediationScript": "Boolean",
  "runSchedule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptRunSchedule"
  },
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "06db0c26-0c26-06db-260c-db06260cdb06",
  "runRemediationScript": "Boolean",
  "runSchedule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptRunSchedule"
  },
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```
