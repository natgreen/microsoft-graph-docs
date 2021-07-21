---
title: "Update unifiedRoleAssignmentScheduleInstance"
description: "Update the properties of an unifiedRoleAssignmentScheduleInstance object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update unifiedRoleAssignmentScheduleInstance
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object.

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
PATCH /roleManagement/directory/roleAssignmentScheduleInstances/{unifiedRoleAssignmentScheduleInstanceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object.

The following table shows the properties that are required when you update the [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appScopeId|String|**TODO: Add Description** Inherited from [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|directoryScopeId|String|**TODO: Add Description** Inherited from [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|principalId|String|**TODO: Add Description** Inherited from [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleDefinitionId|String|**TODO: Add Description** Inherited from [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|assignmentType|String|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|memberType|String|**TODO: Add Description**|
|roleAssignmentOriginId|String|**TODO: Add Description**|
|roleAssignmentScheduleId|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentscheduleinstance"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances/{unifiedRoleAssignmentScheduleInstanceId}
Content-Type: application/json
Content-length: 420

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleInstance",
  "appScopeId": "String",
  "directoryScopeId": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "assignmentType": "String",
  "endDateTime": "String (timestamp)",
  "memberType": "String",
  "roleAssignmentOriginId": "String",
  "roleAssignmentScheduleId": "String",
  "startDateTime": "String (timestamp)"
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
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleInstance",
  "id": "26f51ff3-1ff3-26f5-f31f-f526f31ff526",
  "appScopeId": "String",
  "directoryScopeId": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "assignmentType": "String",
  "endDateTime": "String (timestamp)",
  "memberType": "String",
  "roleAssignmentOriginId": "String",
  "roleAssignmentScheduleId": "String",
  "startDateTime": "String (timestamp)"
}
```
