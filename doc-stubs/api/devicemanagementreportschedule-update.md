---
title: "Update deviceManagementReportSchedule"
description: "Update the properties of a deviceManagementReportSchedule object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceManagementReportSchedule
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.

The following table shows the properties that are required when you update the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|emails|String collection|Emails to which the scheduled reports are delivered|
|endDateTime|DateTimeOffset|Time that the delivery of the scheduled reports ends|
|filter|String|Filters applied on the report|
|format|deviceManagementReportFileFormat|Format of the scheduled report. Possible values are: `csv`, `pdf`.|
|orderBy|String collection|Ordering of columns in the report|
|recurrence|deviceManagementScheduledReportRecurrence|Frequency of scheduled report delivery. Possible values are: `none`, `daily`, `weekly`, `monthly`.|
|reportName|String|Name of the report|
|reportScheduleName|String|Name of the schedule|
|select|String collection|Columns selected from the report|
|startDateTime|DateTimeOffset|Time that the delivery of the scheduled reports starts|
|subject|String|Subject of the scheduled reports that are delivered|
|userId|String|The Id of the User who created the report|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementreportschedule"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
Content-Type: application/json
Content-length: 442

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
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


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "22bc324f-324f-22bc-4f32-bc224f32bc22",
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
