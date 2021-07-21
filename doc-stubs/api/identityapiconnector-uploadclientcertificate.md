---
title: "identityApiConnector: uploadClientCertificate"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# identityApiConnector: uploadClientCertificate
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
POST /identity/apiConnectors/{identityApiConnectorId}/uploadClientCertificate
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
|pkcs12Value|String|**TODO: Add Description**|
|password|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [identityApiConnector](../resources/identityapiconnector.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "identityapiconnector_uploadclientcertificate"
}
-->
``` http
POST https://graph.microsoft.com/beta/identity/apiConnectors/{identityApiConnectorId}/uploadClientCertificate
Content-Type: application/json
Content-length: 56

{
  "pkcs12Value": "String",
  "password": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.identityApiConnector",
    "id": "String (identifier)",
    "authenticationConfiguration": {
      "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
    },
    "displayName": "String",
    "targetUrl": "String"
  }
}
```
