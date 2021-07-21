---
title: "Update smsAuthenticationMethodTarget"
description: "Update the properties of a smsAuthenticationMethodTarget object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update smsAuthenticationMethodTarget
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md) object.

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
PATCH /smsAuthenticationMethodConfiguration/includeTargets/{smsAuthenticationMethodTargetId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md) object.

The following table shows the properties that are required when you update the [smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isRegistrationRequired|Boolean|**TODO: Add Description** Inherited from [authenticationMethodTarget](../resources/authenticationmethodtarget.md)|
|targetType|authenticationMethodTargetType|**TODO: Add Description** Inherited from [authenticationMethodTarget](../resources/authenticationmethodtarget.md). Possible values are: `user`, `group`, `unknownFutureValue`.|
|isUsableForSignIn|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_smsauthenticationmethodtarget"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/smsAuthenticationMethodConfiguration/includeTargets/{smsAuthenticationMethodTargetId}
Content-Type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodTarget",
  "isRegistrationRequired": "Boolean",
  "targetType": "String",
  "isUsableForSignIn": "Boolean"
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
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodTarget",
  "id": "68b1a8ca-a8ca-68b1-caa8-b168caa8b168",
  "isRegistrationRequired": "Boolean",
  "targetType": "String",
  "isUsableForSignIn": "Boolean"
}
```
