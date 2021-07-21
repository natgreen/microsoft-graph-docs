---
title: "Update workbookFormatProtection"
description: "Update the properties of a workbookFormatProtection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update workbookFormatProtection
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [workbookFormatProtection](../resources/workbookformatprotection.md) object.

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
PATCH /workbookFormatProtection
PATCH /workbookRange/format/protection
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookFormatProtection](../resources/workbookformatprotection.md) object.

The following table shows the properties that are required when you update the [workbookFormatProtection](../resources/workbookformatprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|formulaHidden|Boolean|**TODO: Add Description**|
|locked|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookFormatProtection](../resources/workbookformatprotection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_workbookformatprotection"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/workbookFormatProtection
Content-Type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.workbookFormatProtection",
  "formulaHidden": "Boolean",
  "locked": "Boolean"
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
  "@odata.type": "#microsoft.graph.workbookFormatProtection",
  "id": "bd01b1e9-b1e9-bd01-e9b1-01bde9b101bd",
  "formulaHidden": "Boolean",
  "locked": "Boolean"
}
```
