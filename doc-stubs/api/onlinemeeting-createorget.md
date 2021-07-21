---
title: "onlineMeeting: createOrGet"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# onlineMeeting: createOrGet
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
POST /me/onlineMeetings/createOrGet
POST /app/onlineMeetings/createOrGet
POST /communications/onlineMeetings/createOrGet
POST /users/{usersId}/onlineMeetings/createOrGet
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|chatInfo|[chatInfo](../resources/chatinfo.md)|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|participants|[meetingParticipants](../resources/meetingparticipants.md)|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [onlineMeeting](../resources/onlinemeeting.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "onlinemeeting_createorget"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet
Content-Type: application/json
Content-length: 291

{
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo"
  },
  "endDateTime": "String (timestamp)",
  "externalId": "String",
  "participants": {
    "@odata.type": "microsoft.graph.meetingParticipants"
  },
  "startDateTime": "String (timestamp)",
  "subject": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.onlineMeeting",
    "id": "String (identifier)",
    "accessLevel": "String",
    "allowAttendeeToEnableCamera": "Boolean",
    "allowAttendeeToEnableMic": "Boolean",
    "allowedPresenters": "String",
    "allowMeetingChat": "String",
    "allowTeamworkReactions": "Boolean",
    "alternativeRecording": "Stream",
    "attendeeReport": "Stream",
    "audioConferencing": {
      "@odata.type": "microsoft.graph.audioConferencing"
    },
    "broadcastSettings": {
      "@odata.type": "microsoft.graph.broadcastMeetingSettings"
    },
    "canceledDateTime": "String (timestamp)",
    "capabilities": [
      "String"
    ],
    "chatInfo": {
      "@odata.type": "microsoft.graph.chatInfo"
    },
    "creationDateTime": "String (timestamp)",
    "endDateTime": "String (timestamp)",
    "entryExitAnnouncement": "Boolean",
    "expirationDateTime": "String (timestamp)",
    "externalId": "String",
    "isBroadcast": "Boolean",
    "isCancelled": "Boolean",
    "isEntryExitAnnounced": "Boolean",
    "joinInformation": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "joinUrl": "String",
    "lobbyBypassSettings": {
      "@odata.type": "microsoft.graph.lobbyBypassSettings"
    },
    "participants": {
      "@odata.type": "microsoft.graph.meetingParticipants"
    },
    "recording": "Stream",
    "startDateTime": "String (timestamp)",
    "subject": "String",
    "videoTeleconferenceId": "String"
  }
}
```
