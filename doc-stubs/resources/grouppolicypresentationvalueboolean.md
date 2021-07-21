---
title: "groupPolicyPresentationValueBoolean resource type"
description: "The entity represents a Boolean value of a checkbox presentation on a policy definition."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyPresentationValueBoolean resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The entity represents a Boolean value of a checkbox presentation on a policy definition.


Inherits from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationValueBooleans](../api/grouppolicypresentationvalueboolean-list.md)|[groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) collection|Get a list of the [groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) objects and their properties.|
|[Create groupPolicyPresentationValueBoolean](../api/grouppolicypresentationvalueboolean-create.md)|[groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md)|Create a new [groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) object.|
|[Get groupPolicyPresentationValueBoolean](../api/grouppolicypresentationvalueboolean-get.md)|[groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md)|Read the properties and relationships of a [groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) object.|
|[Update groupPolicyPresentationValueBoolean](../api/grouppolicypresentationvalueboolean-update.md)|[groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md)|Update the properties of a [groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) object.|
|[Delete groupPolicyPresentationValueBoolean](../api/grouppolicypresentationvalueboolean-delete.md)|None|Deletes a [groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) object.|
|[List groupPolicyDefinitionValue](../api/grouppolicypresentationvalueboolean-list-definitionvalue.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) collection|Get the groupPolicyDefinitionValue resources from the definitionValue navigation property.|
|[Add groupPolicyDefinitionValue](../api/grouppolicypresentationvalueboolean-post-definitionvalue.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Add definitionValue by posting to the definitionValue collection.|
|[List groupPolicyPresentation](../api/grouppolicypresentationvalueboolean-list-presentation.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md) collection|Get the groupPolicyPresentation resources from the presentation navigation property.|
|[Add groupPolicyPresentation](../api/grouppolicypresentationvalueboolean-post-presentation.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Add presentation by posting to the presentation collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the object was created. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|The date and time the object was last modified. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md).|
|value|Boolean|An boolean value for the associated presentation.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|The group policy definition value associated with the presentation value. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|
|presentation|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|The group policy presentation associated with the presentation value. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueBoolean",
  "baseType": "microsoft.graph.groupPolicyPresentationValue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "value": "Boolean"
}
```
