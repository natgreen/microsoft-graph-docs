---
title: "Update office365ActiveUserCounts"
description: "Update the properties of an office365ActiveUserCounts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update office365ActiveUserCounts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [office365ActiveUserCounts](../resources/office365activeusercounts.md) object.

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
PATCH /office365ActiveUserCounts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [office365ActiveUserCounts](../resources/office365activeusercounts.md) object.

The following table shows the properties that are required when you update the [office365ActiveUserCounts](../resources/office365activeusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|exchange|Int64|**TODO: Add Description**|
|office365|Int64|**TODO: Add Description**|
|oneDrive|Int64|**TODO: Add Description**|
|reportDate|Date|**TODO: Add Description**|
|reportPeriod|String|**TODO: Add Description**|
|reportRefreshDate|Date|**TODO: Add Description**|
|sharePoint|Int64|**TODO: Add Description**|
|skypeForBusiness|Int64|**TODO: Add Description**|
|teams|Int64|**TODO: Add Description**|
|yammer|Int64|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [office365ActiveUserCounts](../resources/office365activeusercounts.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_office365activeusercounts"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/office365ActiveUserCounts
Content-Type: application/json
Content-length: 341

{
  "@odata.type": "#microsoft.graph.office365ActiveUserCounts",
  "exchange": "Integer",
  "office365": "Integer",
  "oneDrive": "Integer",
  "reportDate": "Date",
  "reportPeriod": "String",
  "reportRefreshDate": "Date",
  "sharePoint": "Integer",
  "skypeForBusiness": "Integer",
  "teams": "Integer",
  "yammer": "Integer"
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
  "@odata.type": "#microsoft.graph.office365ActiveUserCounts",
  "id": "0b65939e-939e-0b65-9e93-650b9e93650b",
  "exchange": "Integer",
  "office365": "Integer",
  "oneDrive": "Integer",
  "reportDate": "Date",
  "reportPeriod": "String",
  "reportRefreshDate": "Date",
  "sharePoint": "Integer",
  "skypeForBusiness": "Integer",
  "teams": "Integer",
  "yammer": "Integer"
}
```
