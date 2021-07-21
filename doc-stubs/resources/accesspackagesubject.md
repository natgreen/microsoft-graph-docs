---
title: "accessPackageSubject resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageSubject resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageSubjects](../api/accesspackagesubject-list.md)|[accessPackageSubject](../resources/accesspackagesubject.md) collection|Get a list of the [accessPackageSubject](../resources/accesspackagesubject.md) objects and their properties.|
|[Create accessPackageSubject](../api/accesspackagesubject-create.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Create a new [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Read the properties and relationships of an [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[Update accessPackageSubject](../api/accesspackagesubject-update.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Update the properties of an [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[Delete accessPackageSubject](../api/accesspackagesubject-delete.md)|None|Deletes an [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[List connectedOrganization](../api/accesspackagesubject-list-connectedorganization.md)|[connectedOrganization](../resources/connectedorganization.md) collection|Get the connectedOrganization resources from the connectedOrganization navigation property.|
|[Add connectedOrganization](../api/accesspackagesubject-post-connectedorganization.md)|[connectedOrganization](../resources/connectedorganization.md)|Add connectedOrganization by posting to the connectedOrganization collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|altSecId|String|**TODO: Add Description**|
|connectedOrganizationId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|objectId|String|**TODO: Add Description**|
|onPremisesSecurityIdentifier|String|**TODO: Add Description**|
|principalName|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|connectedOrganization|[connectedOrganization](../resources/connectedorganization.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "id": "String (identifier)",
  "altSecId": "String",
  "connectedOrganizationId": "String",
  "displayName": "String",
  "email": "String",
  "objectId": "String",
  "onPremisesSecurityIdentifier": "String",
  "principalName": "String",
  "type": "String"
}
```
