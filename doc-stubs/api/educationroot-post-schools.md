---
title: "Create educationSchool"
description: "Create a new educationSchool object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create educationSchool
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new educationSchool object.

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
POST /education/schools
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [educationSchool](../resources/educationschool.md) object.

The following table shows the properties that are required when you create the [educationSchool](../resources/educationschool.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description** Inherited from [educationOrganization](../resources/educationorganization.md)|
|displayName|String|**TODO: Add Description** Inherited from [educationOrganization](../resources/educationorganization.md)|
|externalSource|educationExternalSource|**TODO: Add Description** Inherited from [educationOrganization](../resources/educationorganization.md). Possible values are: `sis`, `manual`, `unknownFutureValue`, `lms`.|
|externalSourceDetail|String|**TODO: Add Description** Inherited from [educationOrganization](../resources/educationorganization.md)|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|externalPrincipalId|String|**TODO: Add Description**|
|fax|String|**TODO: Add Description**|
|highestGrade|String|**TODO: Add Description**|
|lowestGrade|String|**TODO: Add Description**|
|phone|String|**TODO: Add Description**|
|principalEmail|String|**TODO: Add Description**|
|principalName|String|**TODO: Add Description**|
|schoolNumber|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/schools
Content-Type: application/json
Content-length: 583

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "description": "String",
  "displayName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "externalId": "String",
  "externalPrincipalId": "String",
  "fax": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "phone": "String",
  "principalEmail": "String",
  "principalName": "String",
  "schoolNumber": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "88382426-2426-8838-2624-388826243888",
  "description": "String",
  "displayName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "externalId": "String",
  "externalPrincipalId": "String",
  "fax": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "phone": "String",
  "principalEmail": "String",
  "principalName": "String",
  "schoolNumber": "String"
}
```
