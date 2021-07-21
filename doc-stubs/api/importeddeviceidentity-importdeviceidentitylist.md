---
title: "importedDeviceIdentity: importDeviceIdentityList"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# importedDeviceIdentity: importDeviceIdentityList
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
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
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
|importedDeviceIdentities|[importedDeviceIdentity](../resources/importeddeviceidentity.md) collection|**TODO: Add Description**|
|overwriteImportedDeviceIdentities|Boolean|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "importeddeviceidentity_importdeviceidentitylist"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList
Content-Type: application/json
Content-length: 551

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "String (identifier)",
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "enrollmentState": "String",
      "importedDeviceIdentifier": "String",
      "importedDeviceIdentityType": "String",
      "lastContactedDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "platform": "String"
    }
  ],
  "overwriteImportedDeviceIdentities": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.importedDeviceIdentityResult)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "String (identifier)",
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "enrollmentState": "String",
      "importedDeviceIdentifier": "String",
      "importedDeviceIdentityType": "String",
      "lastContactedDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "platform": "String",
      "status": "Boolean"
    }
  ]
}
```
