---
title: "managementConditionStatement resource type"
description: "A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managementConditionStatement resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementConditionStatements](../api/managementconditionstatement-list.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection|Get a list of the [managementConditionStatement](../resources/managementconditionstatement.md) objects and their properties.|
|[Create managementConditionStatement](../api/managementconditionstatement-create.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Create a new [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[Get managementConditionStatement](../api/managementconditionstatement-get.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Read the properties and relationships of a [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[Update managementConditionStatement](../api/managementconditionstatement-update.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Update the properties of a [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[Delete managementConditionStatement](../api/managementconditionstatement-delete.md)|None|Deletes a [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[getManagementConditionStatementExpressionString](../api/managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/managementconditionexpressionstring.md)|**TODO: Add Description**|
|[getManagementConditionStatementsForPlatform](../api/managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection|**TODO: Add Description**|
|[List managementConditions](../api/managementconditionstatement-list-managementconditions.md)|[managementCondition](../resources/managementcondition.md) collection|Get the managementCondition resources from the managementConditions navigation property.|
|[Add managementCondition](../api/managementconditionstatement-post-managementconditions.md)|[managementCondition](../resources/managementcondition.md)|Add managementConditions by posting to the managementConditions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|devicePlatformType collection|The applicable platforms for this management condition statement.
This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.|
|createdDateTime|DateTimeOffset|The time the management condition statement was created. Generated service side.|
|description|String|The admin defined description of the management condition statement.|
|displayName|String|The admin defined name of the management condition statement.|
|eTag|String|ETag of the management condition statement. Updated service side.|
|expression|[managementConditionExpression](../resources/managementconditionexpression.md)|The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|modifiedDateTime|DateTimeOffset|The time the management condition statement was last modified. Updated service side.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementConditions|[managementCondition](../resources/managementcondition.md) collection|The management conditions associated to the management condition statement.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "applicablePlatforms": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "eTag": "String",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "modifiedDateTime": "String (timestamp)"
}
```
