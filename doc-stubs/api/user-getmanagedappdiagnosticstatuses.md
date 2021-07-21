---
title: "user: getManagedAppDiagnosticStatuses"
description: "Gets diagnostics validation status for a given user."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# user: getManagedAppDiagnosticStatuses
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gets diagnostics validation status for a given user.

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
GET /me/getManagedAppDiagnosticStatuses
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/managedappdiagnosticstatus.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_getmanagedappdiagnosticstatuses"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/getManagedAppDiagnosticStatuses
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedAppDiagnosticStatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
    }
  ]
}
```
