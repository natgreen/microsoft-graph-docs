---
title: "List deviceShellScripts"
description: "Get the deviceShellScript resources from the deviceShellScripts navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List deviceShellScripts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the deviceShellScript resources from the deviceShellScripts navigation property.

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
GET /deviceManagement/deviceShellScripts
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [deviceShellScript](../resources/deviceshellscript.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_deviceshellscript"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.deviceShellScript)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceShellScript",
      "id": "ee7fef6e-ef6e-ee7f-6eef-7fee6eef7fee",
      "blockExecutionNotifications": "Boolean",
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "displayName": "String",
      "executionFrequency": "String (duration)",
      "fileName": "String",
      "lastModifiedDateTime": "String (timestamp)",
      "retryCount": "Integer",
      "roleScopeTagIds": [
        "String"
      ],
      "runAsAccount": "String",
      "scriptContent": "Binary"
    }
  ]
}
```
