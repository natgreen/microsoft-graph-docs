---
title: "meetingPolicyUpdatedEventMessageDetail resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# meetingPolicyUpdatedEventMessageDetail resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [eventMessageDetail](../resources/eventmessagedetail.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|meetingChatEnabled|Boolean|**TODO: Add Description**|
|meetingChatId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingPolicyUpdatedEventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingPolicyUpdatedEventMessageDetail",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "meetingChatEnabled": "Boolean",
  "meetingChatId": "String"
}
```
