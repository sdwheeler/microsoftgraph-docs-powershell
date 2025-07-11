---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgidentityb2xuserflow
schema: 2.0.0
ms.subservice: entra-sign-in
---

# New-MgIdentityB2XUserFlow

## SYNOPSIS
Create a new b2xIdentityUserFlow object.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaIdentityB2XUserFlow](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/New-MgBetaIdentityB2XUserFlow?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgIdentityB2XUserFlow [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-ApiConnectorConfiguration <IMicrosoftGraphUserFlowApiConnectorConfiguration>] [-Id <String>]
 [-IdentityProviders <IMicrosoftGraphIdentityProvider[]>]
 [-Languages <IMicrosoftGraphUserFlowLanguageConfiguration[]>]
 [-UserAttributeAssignments <IMicrosoftGraphIdentityUserFlowAttributeAssignment[]>]
 [-UserFlowIdentityProviders <IMicrosoftGraphIdentityProviderBase[]>] [-UserFlowType <String>]
 [-UserFlowTypeVersion <Single>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgIdentityB2XUserFlow -BodyParameter <IMicrosoftGraphB2XIdentityUserFlow>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new b2xIdentityUserFlow object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | IdentityUserFlow.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | IdentityUserFlow.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApiConnectorConfiguration
userFlowApiConnectorConfiguration
To construct, see NOTES section for APICONNECTORCONFIGURATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserFlowApiConnectorConfiguration
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
b2xIdentityUserFlow
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphB2XIdentityUserFlow
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Headers
Optional headers that will be added to the request.

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Id
The unique identifier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IdentityProviders
The identity providers included in the user flow.
To construct, see NOTES section for IDENTITYPROVIDERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentityProvider[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Languages
The languages supported for customization within the user flow.
Language customization is enabled by default in self-service sign-up user flow.
You can't create custom languages in self-service sign-up user flows.
To construct, see NOTES section for LANGUAGES properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserFlowLanguageConfiguration[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResponseHeadersVariable
Optional Response Headers Variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: RHV

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserAttributeAssignments
The user attribute assignments included in the user flow.
To construct, see NOTES section for USERATTRIBUTEASSIGNMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentityUserFlowAttributeAssignment[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserFlowIdentityProviders

To construct, see NOTES section for USERFLOWIDENTITYPROVIDERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentityProviderBase[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserFlowType
userFlowType

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserFlowTypeVersion


```yaml
Type: Single
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphB2XIdentityUserFlow
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphB2XIdentityUserFlow
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

APICONNECTORCONFIGURATION `<IMicrosoftGraphUserFlowApiConnectorConfiguration>`: userFlowApiConnectorConfiguration
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[PostAttributeCollection <IMicrosoftGraphIdentityApiConnector>]`: identityApiConnector
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AuthenticationConfiguration <IMicrosoftGraphApiAuthenticationConfigurationBase>]`: apiAuthenticationConfigurationBase
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The name of the API connector.
    - `[TargetUrl <String>]`: The URL of the API endpoint to call.
  - `[PostFederationSignup <IMicrosoftGraphIdentityApiConnector>]`: identityApiConnector

BODYPARAMETER `<IMicrosoftGraphB2XIdentityUserFlow>`: b2xIdentityUserFlow
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[UserFlowType <String>]`: userFlowType
  - `[UserFlowTypeVersion <Single?>]`:
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ApiConnectorConfiguration <IMicrosoftGraphUserFlowApiConnectorConfiguration>]`: userFlowApiConnectorConfiguration
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[PostAttributeCollection <IMicrosoftGraphIdentityApiConnector>]`: identityApiConnector
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AuthenticationConfiguration <IMicrosoftGraphApiAuthenticationConfigurationBase>]`: apiAuthenticationConfigurationBase
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The name of the API connector.
      - `[TargetUrl <String>]`: The URL of the API endpoint to call.
    - `[PostFederationSignup <IMicrosoftGraphIdentityApiConnector>]`: identityApiConnector
  - `[IdentityProviders <IMicrosoftGraphIdentityProvider- `[]`>]`: The identity providers included in the user flow.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ClientId <String>]`: The client ID for the application.
This is the client ID obtained when registering the application with the identity provider.
Required.
Not nullable.
    - `[ClientSecret <String>]`: The client secret for the application.
This is the client secret obtained when registering the application with the identity provider.
This is write-only.
A read operation will return .
Required.
Not nullable.
    - `[Name <String>]`: The display name of the identity provider.
Not nullable.
    - `[Type <String>]`: The identity provider type is a required field.
For B2B scenario: Google, Facebook.
For B2C scenario: Microsoft, Google, Amazon, LinkedIn, Facebook, GitHub, Twitter, Weibo, QQ, WeChat, OpenIDConnect.
Not nullable.
  - `[Languages <IMicrosoftGraphUserFlowLanguageConfiguration- `[]`>]`: The languages supported for customization within the user flow.
Language customization is enabled by default in self-service sign-up user flow.
You can't create custom languages in self-service sign-up user flows.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DefaultPages <IMicrosoftGraphUserFlowLanguagePage- `[]`>]`: Collection of pages with the default content to display in a user flow for a specified language.
This collection doesn't allow any kind of modification.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: The language name to display.
This property is read-only.
    - `[IsEnabled <Boolean?>]`: Indicates whether the language is enabled within the user flow.
    - `[OverridesPages <IMicrosoftGraphUserFlowLanguagePage- `[]`>]`: Collection of pages with the overrides messages to display in a user flow for a specified language.
This collection only allows you to modify the content of the page, any other modification isn't allowed (creation or deletion of pages).
  - `[UserAttributeAssignments <IMicrosoftGraphIdentityUserFlowAttributeAssignment- `[]`>]`: The user attribute assignments included in the user flow.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: The display name of the identityUserFlowAttribute within a user flow.
    - `[IsOptional <Boolean?>]`: Determines whether the identityUserFlowAttribute is optional.
true means the user doesn't have to provide a value.
false means the user can't complete sign-up without providing a value.
    - `[RequiresVerification <Boolean?>]`: Determines whether the identityUserFlowAttribute requires verification, and is only used for verifying the user's phone number or email address.
    - `[UserAttribute <IMicrosoftGraphIdentityUserFlowAttribute>]`: identityUserFlowAttribute
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DataType <String>]`: identityUserFlowAttributeDataType
      - `[Description <String>]`: The description of the user flow attribute that's shown to the user at the time of sign up.
      - `[DisplayName <String>]`: The display name of the user flow attribute.
Supports $filter (eq, ne).
      - `[UserFlowAttributeType <String>]`: identityUserFlowAttributeType
    - `[UserAttributeValues <IMicrosoftGraphUserAttributeValuesItem- `[]`>]`: The input options for the user flow attribute.
Only applicable when the userInputType is radioSingleSelect, dropdownSingleSelect, or checkboxMultiSelect.
      - `[IsDefault <Boolean?>]`: Determines whether the value is set as the default.
      - `[Name <String>]`: The display name of the property displayed to the user in the user flow.
      - `[Value <String>]`: The value that is set when this item is selected.
    - `[UserInputType <String>]`: identityUserFlowAttributeInputType
  - `[UserFlowIdentityProviders <IMicrosoftGraphIdentityProviderBase- `[]`>]`:
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: The display name of the identity provider.

IDENTITYPROVIDERS `<IMicrosoftGraphIdentityProvider- `[]`>`: The identity providers included in the user flow.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ClientId <String>]`: The client ID for the application.
This is the client ID obtained when registering the application with the identity provider.
Required.
Not nullable.
  - `[ClientSecret <String>]`: The client secret for the application.
This is the client secret obtained when registering the application with the identity provider.
This is write-only.
A read operation will return .
Required.
Not nullable.
  - `[Name <String>]`: The display name of the identity provider.
Not nullable.
  - `[Type <String>]`: The identity provider type is a required field.
For B2B scenario: Google, Facebook.
For B2C scenario: Microsoft, Google, Amazon, LinkedIn, Facebook, GitHub, Twitter, Weibo, QQ, WeChat, OpenIDConnect.
Not nullable.

LANGUAGES `<IMicrosoftGraphUserFlowLanguageConfiguration- `[]`>`: The languages supported for customization within the user flow.
Language customization is enabled by default in self-service sign-up user flow.
You can't create custom languages in self-service sign-up user flows.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DefaultPages <IMicrosoftGraphUserFlowLanguagePage- `[]`>]`: Collection of pages with the default content to display in a user flow for a specified language.
This collection doesn't allow any kind of modification.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The language name to display.
This property is read-only.
  - `[IsEnabled <Boolean?>]`: Indicates whether the language is enabled within the user flow.
  - `[OverridesPages <IMicrosoftGraphUserFlowLanguagePage- `[]`>]`: Collection of pages with the overrides messages to display in a user flow for a specified language.
This collection only allows you to modify the content of the page, any other modification isn't allowed (creation or deletion of pages).

USERATTRIBUTEASSIGNMENTS `<IMicrosoftGraphIdentityUserFlowAttributeAssignment- `[]`>`: The user attribute assignments included in the user flow.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The display name of the identityUserFlowAttribute within a user flow.
  - `[IsOptional <Boolean?>]`: Determines whether the identityUserFlowAttribute is optional.
true means the user doesn't have to provide a value.
false means the user can't complete sign-up without providing a value.
  - `[RequiresVerification <Boolean?>]`: Determines whether the identityUserFlowAttribute requires verification, and is only used for verifying the user's phone number or email address.
  - `[UserAttribute <IMicrosoftGraphIdentityUserFlowAttribute>]`: identityUserFlowAttribute
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DataType <String>]`: identityUserFlowAttributeDataType
    - `[Description <String>]`: The description of the user flow attribute that's shown to the user at the time of sign up.
    - `[DisplayName <String>]`: The display name of the user flow attribute.
Supports $filter (eq, ne).
    - `[UserFlowAttributeType <String>]`: identityUserFlowAttributeType
  - `[UserAttributeValues <IMicrosoftGraphUserAttributeValuesItem- `[]`>]`: The input options for the user flow attribute.
Only applicable when the userInputType is radioSingleSelect, dropdownSingleSelect, or checkboxMultiSelect.
    - `[IsDefault <Boolean?>]`: Determines whether the value is set as the default.
    - `[Name <String>]`: The display name of the property displayed to the user in the user flow.
    - `[Value <String>]`: The value that is set when this item is selected.
  - `[UserInputType <String>]`: identityUserFlowAttributeInputType

USERFLOWIDENTITYPROVIDERS `<IMicrosoftGraphIdentityProviderBase- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The display name of the identity provider.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgidentityb2xuserflow](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgidentityb2xuserflow)

[https://learn.microsoft.com/graph/api/identitycontainer-post-b2xuserflows?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/identitycontainer-post-b2xuserflows?view=graph-rest-1.0)
























