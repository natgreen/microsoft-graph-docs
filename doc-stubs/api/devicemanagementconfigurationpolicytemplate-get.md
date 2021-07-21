---
title: "Get deviceManagementConfigurationPolicyTemplate"
description: "Read the properties and relationships of a deviceManagementConfigurationPolicyTemplate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get deviceManagementConfigurationPolicyTemplate
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [deviceManagementConfigurationPolicyTemplate](../resources/devicemanagementconfigurationpolicytemplate.md) object.

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
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}
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

If successful, this method returns a `200 OK` response code and a [deviceManagementConfigurationPolicyTemplate](../resources/devicemanagementconfigurationpolicytemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementconfigurationpolicytemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
    "id": "e59d9aef-9aef-e59d-ef9a-9de5ef9a9de5",
    "allowUnmanagedSettings": "Boolean",
    "baseId": "String",
    "description": "String",
    "displayName": "String",
    "displayVersion": "String",
    "lifecycleState": "String",
    "platforms": "String",
    "settingTemplateCount": "Integer",
    "technologies": "String",
    "templateFamily": "String",
    "version": "Integer"
  }
}
```
