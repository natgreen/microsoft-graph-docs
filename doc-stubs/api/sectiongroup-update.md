---
title: "Update sectionGroup"
description: "Update the properties of a sectionGroup object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update sectionGroup
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [sectionGroup](../resources/sectiongroup.md) object.

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
PATCH /me/onenote/sectionGroups/{sectionGroupId}
PATCH /users/{usersId}/onenote/sectionGroups/{sectionGroupId}
PATCH /me/onenote/notebooks/{notebookId}/sectionGroups/{sectionGroupId}
PATCH /users/{usersId}/onenote/notebooks/{notebookId}/sectionGroups/{sectionGroupId}
PATCH /me/onenote/notebooks/{notebookId}/sectionGroups/{sectionGroupId}/parentSectionGroup
PATCH /me/onenote/notebooks/{notebookId}/sectionGroups/{sectionGroupId}/sectionGroups/{sectionGroupId}
PATCH /users/{usersId}/onenote/notebooks/{notebookId}/sectionGroups/{sectionGroupId}/parentSectionGroup
PATCH /users/{usersId}/onenote/notebooks/{notebookId}/sectionGroups/{sectionGroupId}/sectionGroups/{sectionGroupId}
PATCH /me/onenote/notebooks/{notebookId}/sectionGroups/{sectionGroupId}/sections/{onenoteSectionId}/parentSectionGroup
PATCH /users/{usersId}/onenote/notebooks/{notebookId}/sectionGroups/{sectionGroupId}/sections/{onenoteSectionId}/parentSectionGroup
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [sectionGroup](../resources/sectiongroup.md) object.

The following table shows the properties that are required when you update the [sectionGroup](../resources/sectiongroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|displayName|String|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|sectionGroupsUrl|String|**TODO: Add Description**|
|sectionsUrl|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [sectionGroup](../resources/sectiongroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_sectiongroup"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/onenote/sectionGroups/{sectionGroupId}
Content-Type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.sectionGroup",
  "self": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "displayName": "String",
  "sectionGroupsUrl": "String",
  "sectionsUrl": "String"
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
  "@odata.type": "#microsoft.graph.sectionGroup",
  "id": "48e22c3c-2c3c-48e2-3c2c-e2483c2ce248",
  "self": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "displayName": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "sectionGroupsUrl": "String",
  "sectionsUrl": "String"
}
```
