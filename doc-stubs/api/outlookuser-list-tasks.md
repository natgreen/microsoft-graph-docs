---
title: "List tasks"
description: "Get the outlookTask resources from the tasks navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List tasks
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the outlookTask resources from the tasks navigation property.

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
GET /users/{usersId}/outlook/tasks
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

If successful, this method returns a `200 OK` response code and a collection of [outlookTask](../resources/outlooktask.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_outlooktask"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/outlook/tasks
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.outlookTask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.outlookTask",
      "id": "3a062144-2144-3a06-4421-063a4421063a",
      "categories": [
        "String"
      ],
      "changeKey": "String",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "assignedTo": "String",
      "body": {
        "@odata.type": "microsoft.graph.itemBody"
      },
      "completedDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "dueDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "hasAttachments": "Boolean",
      "importance": "String",
      "isReminderOn": "Boolean",
      "owner": "String",
      "parentFolderId": "String",
      "recurrence": {
        "@odata.type": "microsoft.graph.patternedRecurrence"
      },
      "reminderDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "sensitivity": "String",
      "startDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "status": "String",
      "subject": "String"
    }
  ]
}
```
