---
title: "Update roleAssignment"
description: "Update the properties of a roleAssignment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update roleAssignment
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [roleAssignment](../resources/roleassignment.md) object.

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
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}/roleDefinition/roleAssignments/{roleAssignmentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [roleAssignment](../resources/roleassignment.md) object.

The following table shows the properties that are required when you update the [roleAssignment](../resources/roleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|Description of the Role Assignment.|
|displayName|String|The display or friendly name of the role Assignment.|
|resourceScopes|String collection|List of ids of role scope member security groups. These are IDs from Azure Active Directory.|
|scopeMembers|String collection|List of ids of role scope member security groups. These are IDs from Azure Active Directory.|
|scopeType|roleAssignmentScopeType|Specifies the type of scope for a Role Assignment. Default type 'ResourceScope' allows assignment of ResourceScopes. For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty. Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/roleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_roleassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}/roleDefinition/roleAssignments/{roleAssignmentId}
Content-Type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "description": "String",
  "displayName": "String",
  "resourceScopes": [
    "String"
  ],
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String"
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
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "72860c67-0c67-7286-670c-8672670c8672",
  "description": "String",
  "displayName": "String",
  "resourceScopes": [
    "String"
  ],
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String"
}
```
