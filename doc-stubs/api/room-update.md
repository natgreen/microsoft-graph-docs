---
title: "Update room"
description: "Update the properties of a room object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update room
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [room](../resources/room.md) object.

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
PATCH /room
PATCH /roomList/rooms/{roomId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [room](../resources/room.md) object.

The following table shows the properties that are required when you update the [room](../resources/room.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|displayName|String|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|geoCoordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|phone|String|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|audioDeviceName|String|**TODO: Add Description**|
|bookingType|bookingType|**TODO: Add Description**. Possible values are: `unknown`, `standard`, `reserved`.|
|building|String|**TODO: Add Description**|
|capacity|Int32|**TODO: Add Description**|
|displayDeviceName|String|**TODO: Add Description**|
|emailAddress|String|**TODO: Add Description**|
|floorLabel|String|**TODO: Add Description**|
|floorNumber|Int32|**TODO: Add Description**|
|isWheelChairAccessible|Boolean|**TODO: Add Description**|
|label|String|**TODO: Add Description**|
|nickname|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|videoDeviceName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [room](../resources/room.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_room"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/room
Content-Type: application/json
Content-length: 643

{
  "@odata.type": "#microsoft.graph.room",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "displayName": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "phone": "String",
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": "Integer",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": "Integer",
  "isWheelChairAccessible": "Boolean",
  "label": "String",
  "nickname": "String",
  "tags": [
    "String"
  ],
  "videoDeviceName": "String"
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
  "@odata.type": "#microsoft.graph.room",
  "id": "0ba727ab-27ab-0ba7-ab27-a70bab27a70b",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "displayName": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "phone": "String",
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": "Integer",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": "Integer",
  "isWheelChairAccessible": "Boolean",
  "label": "String",
  "nickname": "String",
  "tags": [
    "String"
  ],
  "videoDeviceName": "String"
}
```
