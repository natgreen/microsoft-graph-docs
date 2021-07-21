---
title: "Update orgContact"
description: "Update the properties of an orgContact object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update orgContact
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [orgContact](../resources/orgcontact.md) object.

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
PATCH /contacts/{contactsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [orgContact](../resources/orgcontact.md) object.

The following table shows the properties that are required when you update the [orgContact](../resources/orgcontact.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|addresses|[physicalOfficeAddress](../resources/physicalofficeaddress.md) collection|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|phones|[phone](../resources/phone.md) collection|**TODO: Add Description**|
|proxyAddresses|String collection|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [orgContact](../resources/orgcontact.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/contacts/{contactsId}
Content-Type: application/json
Content-length: 747

{
  "@odata.type": "#microsoft.graph.orgContact",
  "deletedDateTime": "String (timestamp)",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalOfficeAddress"
    }
  ],
  "companyName": "String",
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "jobTitle": "String",
  "mail": "String",
  "mailNickname": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSyncEnabled": "Boolean",
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "surname": "String"
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
  "@odata.type": "#microsoft.graph.orgContact",
  "id": "c1d48836-8836-c1d4-3688-d4c13688d4c1",
  "deletedDateTime": "String (timestamp)",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalOfficeAddress"
    }
  ],
  "companyName": "String",
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "jobTitle": "String",
  "mail": "String",
  "mailNickname": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSyncEnabled": "Boolean",
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "surname": "String"
}
```
