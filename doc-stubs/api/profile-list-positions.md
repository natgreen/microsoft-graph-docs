---
title: "List positions"
description: "Get the workPosition resources from the positions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List positions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the workPosition resources from the positions navigation property.

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
GET /users/{usersId}/profile/positions
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

If successful, this method returns a `200 OK` response code and a collection of [workPosition](../resources/workposition.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_workposition"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/profile/positions
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.workPosition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workPosition",
      "id": "00e3d246-d246-00e3-46d2-e30046d2e300",
      "allowedAudiences": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "String (timestamp)",
      "inference": {
        "@odata.type": "microsoft.graph.inferenceData"
      },
      "isSearchable": "Boolean",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "source": {
        "@odata.type": "microsoft.graph.personDataSources"
      },
      "categories": [
        "String"
      ],
      "colleagues": [
        {
          "@odata.type": "microsoft.graph.relatedPerson"
        }
      ],
      "detail": {
        "@odata.type": "microsoft.graph.positionDetail"
      },
      "isCurrent": "Boolean",
      "manager": {
        "@odata.type": "microsoft.graph.relatedPerson"
      }
    }
  ]
}
```
