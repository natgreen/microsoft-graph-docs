---
title: "accessReviewSet resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessReviewSet resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessReviewSets](../api/accessreviewset-list.md)|[accessReviewSet](../resources/accessreviewset.md) collection|Get a list of the [accessReviewSet](../resources/accessreviewset.md) objects and their properties.|
|[Create accessReviewSet](../api/accessreviewset-create.md)|[accessReviewSet](../resources/accessreviewset.md)|Create a new [accessReviewSet](../resources/accessreviewset.md) object.|
|[Get accessReviewSet](../api/accessreviewset-get.md)|[accessReviewSet](../resources/accessreviewset.md)|Read the properties and relationships of an [accessReviewSet](../resources/accessreviewset.md) object.|
|[Update accessReviewSet](../api/accessreviewset-update.md)|[accessReviewSet](../resources/accessreviewset.md)|Update the properties of an [accessReviewSet](../resources/accessreviewset.md) object.|
|[Delete accessReviewSet](../api/accessreviewset-delete.md)|None|Deletes an [accessReviewSet](../resources/accessreviewset.md) object.|
|[List definitions](../api/accessreviewset-list-definitions.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) collection|Get the accessReviewScheduleDefinition resources from the definitions navigation property.|
|[Create accessReviewScheduleDefinition](../api/accessreviewset-post-definitions.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Create a new accessReviewScheduleDefinition object.|
|[List historyDefinitions](../api/accessreviewset-list-historydefinitions.md)|[accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) collection|Get the accessReviewHistoryDefinition resources from the historyDefinitions navigation property.|
|[Create accessReviewHistoryDefinition](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md)|Create a new accessReviewHistoryDefinition object.|
|[List accessReviewPolicy](../api/accessreviewset-list-policy.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md) collection|Get the accessReviewPolicy resources from the policy navigation property.|
|[Create accessReviewPolicy](../api/accessreviewset-post-policy.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Create a new accessReviewPolicy object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitions|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) collection|**TODO: Add Description**|
|historyDefinitions|[accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) collection|**TODO: Add Description**|
|policy|[accessReviewPolicy](../resources/accessreviewpolicy.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewSet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewSet",
  "id": "String (identifier)"
}
```
