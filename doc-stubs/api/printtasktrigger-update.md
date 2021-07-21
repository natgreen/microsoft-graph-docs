---
title: "Update printTaskTrigger"
description: "Update the properties of a printTaskTrigger object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update printTaskTrigger
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [printTaskTrigger](../resources/printtasktrigger.md) object.

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
PATCH /print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
PATCH /print/printers/{printerId}/jobs/{printJobId}/tasks/{printTaskId}/trigger
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [printTaskTrigger](../resources/printtasktrigger.md) object.

The following table shows the properties that are required when you update the [printTaskTrigger](../resources/printtasktrigger.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|event|printEvent|**TODO: Add Description**. Possible values are: `jobStarted`, `unknownFutureValue`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [printTaskTrigger](../resources/printtasktrigger.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_printtasktrigger"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
Content-Type: application/json
Content-length: 80

{
  "@odata.type": "#microsoft.graph.printTaskTrigger",
  "event": "String"
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
  "@odata.type": "#microsoft.graph.printTaskTrigger",
  "id": "75556730-6730-7555-3067-557530675575",
  "event": "String"
}
```
