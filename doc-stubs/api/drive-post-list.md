---
title: "Create list"
description: "Create a new list object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create list
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new list object.

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
POST /drive/list
POST /drives/{drivesId}/list
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [list](../resources/list.md) object.

The following table shows the properties that are required when you create the [list](../resources/list.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|description|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|displayName|String|**TODO: Add Description**|
|list|[listInfo](../resources/listinfo.md)|**TODO: Add Description**|
|sharepointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description**|
|system|[systemFacet](../resources/systemfacet.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [list](../resources/list.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_list_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/drive/list
Content-Type: application/json
Content-length: 540

{
  "@odata.type": "#microsoft.graph.list",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": "String",
  "eTag": "String",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "webUrl": "String",
  "displayName": "String",
  "list": {
    "@odata.type": "microsoft.graph.listInfo"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "system": {
    "@odata.type": "microsoft.graph.systemFacet"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.list"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.list",
  "id": "1361015c-015c-1361-5c01-61135c016113",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "eTag": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "webUrl": "String",
  "displayName": "String",
  "list": {
    "@odata.type": "microsoft.graph.listInfo"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "system": {
    "@odata.type": "microsoft.graph.systemFacet"
  }
}
```
