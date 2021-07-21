---
title: "List userExperienceAnalyticsDeviceStartupHistory"
description: "Get the userExperienceAnalyticsDeviceStartupHistory resources from the userExperienceAnalyticsDeviceStartupHistory navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List userExperienceAnalyticsDeviceStartupHistory
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the userExperienceAnalyticsDeviceStartupHistory resources from the userExperienceAnalyticsDeviceStartupHistory navigation property.

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
GET /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
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

If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_userexperienceanalyticsdevicestartuphistory"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userExperienceAnalyticsDeviceStartupHistory)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
      "id": "5e7ef792-f792-5e7e-92f7-7e5e92f77e5e",
      "coreBootTimeInMs": "Integer",
      "coreLoginTimeInMs": "Integer",
      "deviceId": "String",
      "featureUpdateBootTimeInMs": "Integer",
      "groupPolicyBootTimeInMs": "Integer",
      "groupPolicyLoginTimeInMs": "Integer",
      "isFeatureUpdate": "Boolean",
      "isFirstLogin": "Boolean",
      "operatingSystemVersion": "String",
      "responsiveDesktopTimeInMs": "Integer",
      "restartCategory": "String",
      "restartFaultBucket": "String",
      "restartStopCode": "String",
      "startTime": "String (timestamp)",
      "totalBootTimeInMs": "Integer",
      "totalLoginTimeInMs": "Integer"
    }
  ]
}
```
