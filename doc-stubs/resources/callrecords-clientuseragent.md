---
title: "clientUserAgent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# clientUserAgent resource type

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [userAgent](../resources/callrecords-useragent.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationVersion|String|**TODO: Add Description** Inherited from [userAgent](../resources/callrecords-useragent.md).|
|headerValue|String|**TODO: Add Description** Inherited from [userAgent](../resources/callrecords-useragent.md).|
|platform|clientPlatform|**TODO: Add Description**. Possible values are: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.|
|productFamily|productFamily|**TODO: Add Description**. Possible values are: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.clientUserAgent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
  "applicationVersion": "String",
  "headerValue": "String",
  "platform": "String",
  "productFamily": "String"
}
```
