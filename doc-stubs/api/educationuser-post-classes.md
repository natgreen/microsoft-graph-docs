---
title: "Add educationClass"
description: "Add classes by posting to the classes collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add educationClass
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add classes by posting to the classes collection.

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
POST /education/classes/{educationClassId}/members/{educationUserId}/classes/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [educationClass](../resources/educationclass.md) object.

The following table shows the properties that are required when you create the [educationClass](../resources/educationclass.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|classCode|String|**TODO: Add Description**|
|course|[educationCourse](../resources/educationcourse.md)|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|externalName|String|**TODO: Add Description**|
|externalSource|educationExternalSource|**TODO: Add Description**. Possible values are: `sis`, `manual`, `unknownFutureValue`, `lms`.|
|externalSourceDetail|String|**TODO: Add Description**|
|grade|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|term|[educationTerm](../resources/educationterm.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/members/{educationUserId}/classes/$ref
Content-Type: application/json
Content-length: 533

{
  "@odata.type": "#microsoft.graph.educationClass",
  "classCode": "String",
  "course": {
    "@odata.type": "microsoft.graph.educationCourse"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "mailNickname": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "b4e92fab-2fab-b4e9-ab2f-e9b4ab2fe9b4",
  "classCode": "String",
  "course": {
    "@odata.type": "microsoft.graph.educationCourse"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "mailNickname": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
