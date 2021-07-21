---
title: "swapShiftsChangeRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# swapShiftsChangeRequest resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [offerShiftRequest](../resources/offershiftrequest.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List swapShiftsChangeRequests](../api/swapshiftschangerequest-list.md)|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) collection|Get a list of the [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) objects and their properties.|
|[Create swapShiftsChangeRequest](../api/swapshiftschangerequest-create.md)|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)|Create a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.|
|[Get swapShiftsChangeRequest](../api/swapshiftschangerequest-get.md)|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)|Read the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.|
|[Update swapShiftsChangeRequest](../api/swapshiftschangerequest-update.md)|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)|Update the properties of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.|
|[Delete swapShiftsChangeRequest](../api/swapshiftschangerequest-delete.md)|None|Deletes a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedTo|scheduleChangeRequestActor|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md).|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md).|
|managerActionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md).|
|managerActionMessage|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md).|
|managerUserId|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md).|
|recipientActionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [offerShiftRequest](../resources/offershiftrequest.md).|
|recipientActionMessage|String|**TODO: Add Description** Inherited from [offerShiftRequest](../resources/offershiftrequest.md).|
|recipientShiftId|String|**TODO: Add Description**|
|recipientUserId|String|**TODO: Add Description** Inherited from [offerShiftRequest](../resources/offershiftrequest.md).|
|senderDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md).|
|senderMessage|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md).|
|senderShiftId|String|**TODO: Add Description** Inherited from [offerShiftRequest](../resources/offershiftrequest.md).|
|senderUserId|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md).|
|state|scheduleChangeState|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest",
  "baseType": "microsoft.graph.offerShiftRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.swapShiftsChangeRequest",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "assignedTo": "String",
  "managerActionDateTime": "String (timestamp)",
  "managerActionMessage": "String",
  "managerUserId": "String",
  "senderDateTime": "String (timestamp)",
  "senderMessage": "String",
  "senderUserId": "String",
  "state": "String",
  "recipientActionDateTime": "String (timestamp)",
  "recipientActionMessage": "String",
  "recipientUserId": "String",
  "senderShiftId": "String",
  "recipientShiftId": "String"
}
```
