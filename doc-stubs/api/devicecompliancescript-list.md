---
title: "List deviceComplianceScripts"
description: "Get a list of the deviceComplianceScript objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List deviceComplianceScripts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [deviceComplianceScript](../resources/devicecompliancescript.md) objects and their properties.

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
GET /deviceManagement/deviceComplianceScripts
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

If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScript](../resources/devicecompliancescript.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_devicecompliancescript"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.deviceComplianceScript)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScript",
      "id": "d7f36754-6754-d7f3-5467-f3d75467f3d7",
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "detectionScriptContent": "Binary",
      "displayName": "String",
      "enforceSignatureCheck": "Boolean",
      "lastModifiedDateTime": "String (timestamp)",
      "publisher": "String",
      "roleScopeTagIds": [
        "String"
      ],
      "runAs32Bit": "Boolean",
      "runAsAccount": "String",
      "version": "String"
    }
  ]
}
```
