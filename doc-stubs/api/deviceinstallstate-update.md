---
title: "Update deviceInstallState"
description: "Update the properties of a deviceInstallState object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceInstallState
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [deviceInstallState](../resources/deviceinstallstate.md) object.

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
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceInstallState](../resources/deviceinstallstate.md) object.

The following table shows the properties that are required when you update the [deviceInstallState](../resources/deviceinstallstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deviceId|String|Device Id.|
|deviceName|String|Device name.|
|errorCode|String|The error code for install failures.|
|installState|installState|The install state of the eBook. Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.|
|lastSyncDateTime|DateTimeOffset|Last sync date and time.|
|osDescription|String|OS Description.|
|osVersion|String|OS Version.|
|userName|String|Device User Name.|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/deviceinstallstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_deviceinstallstate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-Type: application/json
Content-length: 293

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceId": "String",
  "deviceName": "String",
  "errorCode": "String",
  "installState": "String",
  "lastSyncDateTime": "String (timestamp)",
  "osDescription": "String",
  "osVersion": "String",
  "userName": "String"
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
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "123e77ba-77ba-123e-ba77-3e12ba773e12",
  "deviceId": "String",
  "deviceName": "String",
  "errorCode": "String",
  "installState": "String",
  "lastSyncDateTime": "String (timestamp)",
  "osDescription": "String",
  "osVersion": "String",
  "userName": "String"
}
```
