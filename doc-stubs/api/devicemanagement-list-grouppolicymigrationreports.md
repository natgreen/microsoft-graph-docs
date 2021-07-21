---
title: "List groupPolicyMigrationReports"
description: "Get the groupPolicyMigrationReport resources from the groupPolicyMigrationReports navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List groupPolicyMigrationReports
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the groupPolicyMigrationReport resources from the groupPolicyMigrationReports navigation property.

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
GET /deviceManagement/groupPolicyMigrationReports
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

If successful, this method returns a `200 OK` response code and a collection of [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_grouppolicymigrationreport"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.groupPolicyMigrationReport)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
      "id": "3143c08f-c08f-3143-8fc0-43318fc04331",
      "createdDateTime": "String (timestamp)",
      "displayName": "String",
      "groupPolicyCreatedDateTime": "String (timestamp)",
      "groupPolicyLastModifiedDateTime": "String (timestamp)",
      "groupPolicyObjectId": "Guid",
      "lastModifiedDateTime": "String (timestamp)",
      "migrationReadiness": "String",
      "ouDistinguishedName": "String",
      "supportedSettingsCount": "Integer",
      "supportedSettingsPercent": "Integer",
      "targetedInActiveDirectory": "Boolean",
      "totalSettingsCount": "Integer"
    }
  ]
}
```
