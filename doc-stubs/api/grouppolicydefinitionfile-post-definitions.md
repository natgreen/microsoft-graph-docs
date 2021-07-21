---
title: "Add groupPolicyDefinition"
description: "Add definitions by posting to the definitions collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add groupPolicyDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add definitions by posting to the definitions collection.

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
POST /deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}/definitionFile/definitions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.

The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/grouppolicydefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|categoryPath|String|The localized full category path for the policy.|
|classType|groupPolicyDefinitionClassType|Identifies the type of groups the policy can be applied to. Possible values are: `user`, `machine`.|
|displayName|String|The localized policy name.|
|explainText|String|The localized explanation or help text associated with the policy. The default value is empty.|
|groupPolicyCategoryId|Guid|The category id of the parent category|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|
|policyType|groupPolicyType|Specifies the type of group policy. Possible values are: `admxBacked`, `admxIngested`.|
|supportedOn|String|Localized string used to specify what operating system or application version is affected by the policy.|



## Response

If successful, this method returns a `204 No Content` response code and a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_grouppolicydefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}/definitionFile/definitions/$ref
Content-Type: application/json
Content-length: 265

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "categoryPath": "String",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "groupPolicyCategoryId": "Guid",
  "policyType": "String",
  "supportedOn": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "id": "9133657d-657d-9133-7d65-33917d653391",
  "categoryPath": "String",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "groupPolicyCategoryId": "Guid",
  "lastModifiedDateTime": "String (timestamp)",
  "policyType": "String",
  "supportedOn": "String"
}
```
