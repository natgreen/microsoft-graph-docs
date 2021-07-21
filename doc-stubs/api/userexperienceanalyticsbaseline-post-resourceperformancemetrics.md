---
title: "Add userExperienceAnalyticsCategory"
description: "Add resourcePerformanceMetrics by posting to the resourcePerformanceMetrics collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add userExperienceAnalyticsCategory
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add resourcePerformanceMetrics by posting to the resourcePerformanceMetrics collection.

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
POST /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/resourcePerformanceMetrics/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|insights|[userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection|The insights for the user experience analytics category.|



## Response

If successful, this method returns a `204 No Content` response code and a [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticscategory_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/resourcePerformanceMetrics/$ref
Content-Type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "b8c542e1-42e1-b8c5-e142-c5b8e142c5b8",
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
    }
  ]
}
```
