---
title: "educationAssignment: setUpResourcesFolder"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# educationAssignment: setUpResourcesFolder
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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/setUpResourcesFolder
GET /education/classes/{educationClassId}/members/{educationUserId}/assignments/{educationAssignmentId}/setUpResourcesFolder
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [educationAssignment](../resources/educationassignment.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "educationassignment_setupresourcesfolder"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/setUpResourcesFolder
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationAssignment",
    "id": "String (identifier)",
    "addedStudentAction": "String",
    "addToCalendarAction": "String",
    "allowLateSubmissions": "Boolean",
    "allowStudentsToAddResourcesToSubmission": "Boolean",
    "assignDateTime": "String (timestamp)",
    "assignedDateTime": "String (timestamp)",
    "assignTo": {
      "@odata.type": "microsoft.graph.educationAssignmentRecipient"
    },
    "classId": "String",
    "closeDateTime": "String (timestamp)",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "createdDateTime": "String (timestamp)",
    "displayName": "String",
    "dueDateTime": "String (timestamp)",
    "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentGradeType"
    },
    "instructions": {
      "@odata.type": "microsoft.graph.educationItemBody"
    },
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "notificationChannelUrl": "String",
    "resourcesFolderUrl": "String",
    "status": "String",
    "webUrl": "String"
  }
}
```
