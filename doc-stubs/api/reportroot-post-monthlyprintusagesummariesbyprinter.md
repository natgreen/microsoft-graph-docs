---
title: "Create printUsageByPrinter"
description: "Create a new printUsageByPrinter object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create printUsageByPrinter
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new printUsageByPrinter object.

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
POST /reports/monthlyPrintUsageSummariesByPrinter
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [printUsageByPrinter](../resources/printusagebyprinter.md) object.

The following table shows the properties that are required when you create the [printUsageByPrinter](../resources/printusagebyprinter.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|completedBlackAndWhiteJobCount|Int64|**TODO: Add Description** Inherited from [printUsage](../resources/printusage.md)|
|completedColorJobCount|Int64|**TODO: Add Description** Inherited from [printUsage](../resources/printusage.md)|
|incompleteJobCount|Int64|**TODO: Add Description** Inherited from [printUsage](../resources/printusage.md)|
|usageDate|Date|**TODO: Add Description** Inherited from [printUsage](../resources/printusage.md)|
|printerId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [printUsageByPrinter](../resources/printusagebyprinter.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_printusagebyprinter_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/reports/monthlyPrintUsageSummariesByPrinter
Content-Type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.printUsageByPrinter",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "usageDate": "Date",
  "printerId": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByPrinter"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.printUsageByPrinter",
  "id": "3357a57b-a57b-3357-7ba5-57337ba55733",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "usageDate": "Date",
  "printerId": "String"
}
```
