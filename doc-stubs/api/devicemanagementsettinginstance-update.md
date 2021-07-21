---
title: "Update deviceManagementSettingInstance"
description: "Update the properties of a deviceManagementSettingInstance object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceManagementSettingInstance
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.

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
PATCH /deviceManagementComplexSettingInstance/value/{deviceManagementSettingInstanceId}
PATCH /deviceManagementCollectionSettingInstance/value/{deviceManagementSettingInstanceId}
PATCH /deviceManagementAbstractComplexSettingInstance/value/{deviceManagementSettingInstanceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.

The following table shows the properties that are required when you update the [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|definitionId|String|The ID of the setting definition for this instance|
|valueJson|String|JSON representation of the value|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementsettinginstance"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagementComplexSettingInstance/value/{deviceManagementSettingInstanceId}
Content-Type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "definitionId": "String",
  "valueJson": "String"
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
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "e852b26c-b26c-e852-6cb2-52e86cb252e8",
  "definitionId": "String",
  "valueJson": "String"
}
```
