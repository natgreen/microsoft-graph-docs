---
title: "attendeeAvailability resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# attendeeAvailability resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attendee|[attendeeBase](../resources/attendeebase.md)|**TODO: Add Description**|
|availability|freeBusyStatus|**TODO: Add Description**. Possible values are: `unknown`, `free`, `tentative`, `busy`, `oof`, `workingElsewhere`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attendeeAvailability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attendeeAvailability",
  "attendee": {
    "@odata.type": "microsoft.graph.attendeeBase"
  },
  "availability": "String"
}
```
