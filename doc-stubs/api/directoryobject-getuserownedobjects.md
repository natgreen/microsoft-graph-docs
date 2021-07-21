---
title: "directoryObject: getUserOwnedObjects"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# directoryObject: getUserOwnedObjects
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
POST /directoryObjects/getUserOwnedObjects
POST /stsPolicy/appliesTo/getUserOwnedObjects
POST /directory/deletedItems/getUserOwnedObjects
POST /groups/{groupsId}/owners/getUserOwnedObjects
POST /groups/{groupsId}/members/getUserOwnedObjects
POST /groups/{groupsId}/memberOf/getUserOwnedObjects
POST /groups/{groupsId}/acceptedSenders/getUserOwnedObjects
POST /groups/{groupsId}/rejectedSenders/getUserOwnedObjects
POST /groups/{groupsId}/transitiveMembers/getUserOwnedObjects
POST /groups/{groupsId}/transitiveMemberOf/getUserOwnedObjects
POST /domains/{domainsId}/domainNameReferences/getUserOwnedObjects
POST /directoryRoles/{directoryRolesId}/members/getUserOwnedObjects
POST /groups/{groupsId}/membersWithLicenseErrors/getUserOwnedObjects
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
|userId|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "directoryobject_getuserownedobjects"
}
-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/getUserOwnedObjects
Content-Type: application/json
Content-length: 47

{
  "userId": "String",
  "type": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.directoryObject",
    "id": "String (identifier)",
    "deletedDateTime": "String (timestamp)"
  }
}
```
