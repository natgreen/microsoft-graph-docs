---
title: "Update calendarPermission"
description: "Update the properties of a calendarPermission object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update calendarPermission
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [calendarPermission](../resources/calendarpermission.md) object.

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
PATCH /me/calendar/calendarPermissions/{calendarPermissionId}
PATCH /users/{usersId}/calendar/calendarPermissions/{calendarPermissionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [calendarPermission](../resources/calendarpermission.md) object.

The following table shows the properties that are required when you update the [calendarPermission](../resources/calendarpermission.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|allowedRoles|calendarRoleType collection|**TODO: Add Description**. Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description**|
|isInsideOrganization|Boolean|**TODO: Add Description**|
|isRemovable|Boolean|**TODO: Add Description**|
|role|calendarRoleType|**TODO: Add Description**. Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_calendarpermission"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/calendar/calendarPermissions/{calendarPermissionId}
Content-Type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.calendarPermission",
  "allowedRoles": [
    "String"
  ],
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "isInsideOrganization": "Boolean",
  "isRemovable": "Boolean",
  "role": "String"
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
  "@odata.type": "#microsoft.graph.calendarPermission",
  "id": "5e36c544-c544-5e36-44c5-365e44c5365e",
  "allowedRoles": [
    "String"
  ],
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "isInsideOrganization": "Boolean",
  "isRemovable": "Boolean",
  "role": "String"
}
```
