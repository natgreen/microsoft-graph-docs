---
title: "administrativeUnit resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# administrativeUnit resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List administrativeUnits](../api/administrativeunit-list.md)|[administrativeUnit](../resources/administrativeunit.md) collection|Get a list of the [administrativeUnit](../resources/administrativeunit.md) objects and their properties.|
|[Create administrativeUnit](../api/administrativeunit-post-administrativeunits.md)|[administrativeUnit](../resources/administrativeunit.md)|Create a new [administrativeUnit](../resources/administrativeunit.md) object.|
|[Get administrativeUnit](../api/administrativeunit-get.md)|[administrativeUnit](../resources/administrativeunit.md)|Read the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.|
|[Update administrativeUnit](../api/administrativeunit-update.md)|[administrativeUnit](../resources/administrativeunit.md)|Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.|
|[Delete administrativeUnit](../api/administrativeunit-delete.md)|None|Deletes an [administrativeUnit](../resources/administrativeunit.md) object.|
|[checkMemberGroups](../api/administrativeunit-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/administrativeunit-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/administrativeunit-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/administrativeunit-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/administrativeunit-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[delta](../api/administrativeunit-delta.md)|[administrativeUnit](../resources/administrativeunit.md) collection|**TODO: Add Description**|
|[List extensions](../api/administrativeunit-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extension resources from the extensions navigation property.|
|[Create extension](../api/administrativeunit-post-extensions.md)|[extension](../resources/extension.md)|Create a new extension object.|
|[List members](../api/administrativeunit-list-members.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the members navigation property.|
|[Add members](../api/administrativeunit-post-members.md)|[directoryObject](../resources/directoryobject.md)|Add members by posting to the members collection.|
|[List scopedRoleMembers](../api/administrativeunit-list-scopedrolemembers.md)|[scopedRoleMembership](../resources/scopedrolemembership.md) collection|Get the scopedRoleMembership resources from the scopedRoleMembers navigation property.|
|[Create scopedRoleMembership](../api/administrativeunit-post-scopedrolemembers.md)|[scopedRoleMembership](../resources/scopedrolemembership.md)|Create a new scopedRoleMembership object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md).|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|visibility|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|extensions|[extension](../resources/extension.md) collection|**TODO: Add Description**|
|members|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|scopedRoleMembers|[scopedRoleMembership](../resources/scopedrolemembership.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.administrativeUnit",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "visibility": "String"
}
```
