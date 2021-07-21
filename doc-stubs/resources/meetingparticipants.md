---
title: "meetingParticipants resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# meetingParticipants resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attendees|[meetingParticipantInfo](../resources/meetingparticipantinfo.md) collection|**TODO: Add Description**|
|contributors|[meetingParticipantInfo](../resources/meetingparticipantinfo.md) collection|**TODO: Add Description**|
|organizer|[meetingParticipantInfo](../resources/meetingparticipantinfo.md)|**TODO: Add Description**|
|producers|[meetingParticipantInfo](../resources/meetingparticipantinfo.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingParticipants"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingParticipants",
  "attendees": [
    {
      "@odata.type": "microsoft.graph.meetingParticipantInfo"
    }
  ],
  "contributors": [
    {
      "@odata.type": "microsoft.graph.meetingParticipantInfo"
    }
  ],
  "organizer": {
    "@odata.type": "microsoft.graph.meetingParticipantInfo"
  },
  "producers": [
    {
      "@odata.type": "microsoft.graph.meetingParticipantInfo"
    }
  ]
}
```
