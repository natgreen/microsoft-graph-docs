---
title: "accessPackageAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageAssignment resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageAssignments](../api/accesspackageassignment-list.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|Get a list of the [accessPackageAssignment](../resources/accesspackageassignment.md) objects and their properties.|
|[Create accessPackageAssignment](../api/accesspackageassignment-create.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Create a new [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Get accessPackageAssignment](../api/accesspackageassignment-get.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Read the properties and relationships of an [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Update accessPackageAssignment](../api/accesspackageassignment-update.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Update the properties of an [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Delete accessPackageAssignment](../api/accesspackageassignment-delete.md)|None|Deletes an [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|**TODO: Add Description**|
|[List accessPackage](../api/accesspackageassignment-list-accesspackage.md)|[accessPackage](../resources/accesspackage.md) collection|Get the accessPackage resources from the accessPackage navigation property.|
|[Create accessPackage](../api/accesspackageassignment-post-accesspackage.md)|[accessPackage](../resources/accesspackage.md)|Create a new accessPackage object.|
|[List accessPackageAssignmentPolicy](../api/accesspackageassignment-list-accesspackageassignmentpolicy.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) collection|Get the accessPackageAssignmentPolicy resources from the accessPackageAssignmentPolicy navigation property.|
|[Create accessPackageAssignmentPolicy](../api/accesspackageassignment-post-accesspackageassignmentpolicy.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Create a new accessPackageAssignmentPolicy object.|
|[List accessPackageAssignmentRequests](../api/accesspackageassignment-list-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|Get the accessPackageAssignmentRequest resources from the accessPackageAssignmentRequests navigation property.|
|[Create accessPackageAssignmentRequest](../api/accesspackageassignment-post-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Create a new accessPackageAssignmentRequest object.|
|[List accessPackageAssignmentResourceRoles](../api/accesspackageassignment-list-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) collection|Get the accessPackageAssignmentResourceRole resources from the accessPackageAssignmentResourceRoles navigation property.|
|[Create accessPackageAssignmentResourceRole](../api/accesspackageassignment-post-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)|Create a new accessPackageAssignmentResourceRole object.|
|[List accessPackageSubject](../api/accesspackageassignment-list-target.md)|[accessPackageSubject](../resources/accesspackagesubject.md) collection|Get the accessPackageSubject resources from the target navigation property.|
|[Create accessPackageSubject](../api/accesspackageassignment-post-target.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Create a new accessPackageSubject object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessPackageId|String|**TODO: Add Description**|
|assignmentPolicyId|String|**TODO: Add Description**|
|assignmentState|String|**TODO: Add Description**|
|assignmentStatus|String|**TODO: Add Description**|
|catalogId|String|**TODO: Add Description**|
|expiredDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|isExtended|Boolean|**TODO: Add Description**|
|schedule|[requestSchedule](../resources/requestschedule.md)|**TODO: Add Description**|
|targetId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|**TODO: Add Description**|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|**TODO: Add Description**|
|accessPackageAssignmentRequests|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|**TODO: Add Description**|
|accessPackageAssignmentResourceRoles|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) collection|**TODO: Add Description**|
|target|[accessPackageSubject](../resources/accesspackagesubject.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "id": "String (identifier)",
  "accessPackageId": "String",
  "assignmentPolicyId": "String",
  "assignmentState": "String",
  "assignmentStatus": "String",
  "catalogId": "String",
  "expiredDateTime": "String (timestamp)",
  "isExtended": "Boolean",
  "schedule": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "targetId": "String"
}
```
