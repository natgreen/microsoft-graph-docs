---
title: "privilegedSignupStatus: completeSetup"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# privilegedSignupStatus: completeSetup
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
POST /privilegedSignupStatus/completeSetup
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
|tenantSetupInfo|[tenantSetupInfo](../resources/tenantsetupinfo.md)|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [roleSuccessStatistics](../resources/rolesuccessstatistics.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "privilegedsignupstatus_completesetup"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedSignupStatus/completeSetup
Content-Type: application/json
Content-length: 306

{
  "tenantSetupInfo": {
    "@odata.type": "#microsoft.graph.tenantSetupInfo",
    "id": "String (identifier)",
    "firstTimeSetup": "Boolean",
    "relevantRolesSettings": [
      "String"
    ],
    "setupStatus": "String",
    "skipSetup": "Boolean",
    "userRolesActions": "String"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.roleSuccessStatistics)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "microsoft.graph.roleSuccessStatistics"
    }
  ]
}
```
