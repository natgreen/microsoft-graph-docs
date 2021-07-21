---
title: "user: findMeetingTimes"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# user: findMeetingTimes
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
POST /me/findMeetingTimes
POST /users/{usersId}/findMeetingTimes
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
|attendees|[attendeeBase](../resources/attendeebase.md) collection|**TODO: Add Description**|
|locationConstraint|[locationConstraint](../resources/locationconstraint.md)|**TODO: Add Description**|
|timeConstraint|[timeConstraint](../resources/timeconstraint.md)|**TODO: Add Description**|
|meetingDuration|Duration|**TODO: Add Description**|
|maxCandidates|Int32|**TODO: Add Description**|
|isOrganizerOptional|Boolean|**TODO: Add Description**|
|returnSuggestionReasons|Boolean|**TODO: Add Description**|
|minimumAttendeePercentage|Double|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/findMeetingTimes
Content-Type: application/json
Content-length: 460

{
  "attendees": [
    {
      "@odata.type": "microsoft.graph.attendeeBase"
    }
  ],
  "locationConstraint": {
    "@odata.type": "microsoft.graph.locationConstraint"
  },
  "timeConstraint": {
    "@odata.type": "microsoft.graph.timeConstraint"
  },
  "meetingDuration": "String (duration)",
  "maxCandidates": "Integer",
  "isOrganizerOptional": "Boolean",
  "returnSuggestionReasons": "Boolean",
  "minimumAttendeePercentage": "Double"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
  }
}
```
