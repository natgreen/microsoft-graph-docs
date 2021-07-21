---
title: "educationSubmissionResource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationSubmissionResource resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List educationSubmissionResources](../api/educationsubmissionresource-list.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md) collection|Get a list of the [educationSubmissionResource](../resources/educationsubmissionresource.md) objects and their properties.|
|[Create educationSubmissionResource](../api/educationsubmissionresource-create.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Create a new [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|
|[Get educationSubmissionResource](../api/educationsubmissionresource-get.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Read the properties and relationships of an [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|
|[Update educationSubmissionResource](../api/educationsubmissionresource-update.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Update the properties of an [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|
|[Delete educationSubmissionResource](../api/educationsubmissionresource-delete.md)|None|Deletes an [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentResourceUrl|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|resource|[educationResource](../resources/educationresource.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSubmissionResource",
  "id": "String (identifier)",
  "assignmentResourceUrl": "String",
  "resource": {
    "@odata.type": "microsoft.graph.educationResource"
  }
}
```
