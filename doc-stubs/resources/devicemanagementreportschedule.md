---
title: "deviceManagementReportSchedule resource type"
description: "Entity representing a schedule for which reports are delivered"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementReportSchedule resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entity representing a schedule for which reports are delivered


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceManagementReportSchedules](../api/devicemanagementreportschedule-list.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) collection|Get a list of the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) objects and their properties.|
|[Create deviceManagementReportSchedule](../api/devicemanagementreportschedule-create.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Create a new [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.|
|[Get deviceManagementReportSchedule](../api/devicemanagementreportschedule-get.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Read the properties and relationships of a [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.|
|[Update deviceManagementReportSchedule](../api/devicemanagementreportschedule-update.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Update the properties of a [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.|
|[Delete deviceManagementReportSchedule](../api/devicemanagementreportschedule-delete.md)|None|Deletes a [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emails|String collection|Emails to which the scheduled reports are delivered|
|endDateTime|DateTimeOffset|Time that the delivery of the scheduled reports ends|
|filter|String|Filters applied on the report|
|format|deviceManagementReportFileFormat|Format of the scheduled report. Possible values are: `csv`, `pdf`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|orderBy|String collection|Ordering of columns in the report|
|recurrence|deviceManagementScheduledReportRecurrence|Frequency of scheduled report delivery. Possible values are: `none`, `daily`, `weekly`, `monthly`.|
|reportName|String|Name of the report|
|reportScheduleName|String|Name of the schedule|
|select|String collection|Columns selected from the report|
|startDateTime|DateTimeOffset|Time that the delivery of the scheduled reports starts|
|subject|String|Subject of the scheduled reports that are delivered|
|userId|String|The Id of the User who created the report|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReportSchedule",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "String (identifier)",
  "emails": [
    "String"
  ],
  "endDateTime": "String (timestamp)",
  "filter": "String",
  "format": "String",
  "orderBy": [
    "String"
  ],
  "recurrence": "String",
  "reportName": "String",
  "reportScheduleName": "String",
  "select": [
    "String"
  ],
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "userId": "String"
}
```
