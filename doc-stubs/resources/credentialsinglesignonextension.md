---
title: "credentialSingleSignOnExtension resource type"
description: "Represents a Credential-type Single Sign-On extension profile."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# credentialSingleSignOnExtension resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a Credential-type Single Sign-On extension profile.


Inherits from [singleSignOnExtension](../resources/singlesignonextension.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurations|[keyTypedValuePair](../resources/keytypedvaluepair.md) collection|Gets or sets a list of typed key-value pairs used to configure Credential-type profiles. This collection can contain a maximum of 500 elements.|
|domains|String collection|Gets or sets a list of hosts or domain names for which the app extension performs SSO.|
|extensionIdentifier|String|Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.|
|realm|String|Gets or sets the case-sensitive realm name for this profile.|
|teamIdentifier|String|Gets or sets the team ID of the app extension that performs SSO for the specified URLs.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.credentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialSingleSignOnExtension",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyBooleanValuePair"
    }
  ],
  "domains": [
    "String"
  ],
  "extensionIdentifier": "String",
  "realm": "String",
  "teamIdentifier": "String"
}
```
