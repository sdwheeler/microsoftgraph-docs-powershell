---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgidentityauthenticationeventflow
schema: 2.0.0
ms.subservice: entra-sign-in
---

# Update-MgIdentityAuthenticationEventFlow

## SYNOPSIS
Update the properties of an authenticationEventsFlow object by ID.
You must specify the @odata.type property and the value of the authenticationEventsFlow object type to update.
The following derived subtypes are supported:- externalUsersSelfServiceSignupEventsFlow

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaIdentityAuthenticationEventFlow](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/Update-MgBetaIdentityAuthenticationEventFlow?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgIdentityAuthenticationEventFlow -AuthenticationEventsFlowId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Conditions <IMicrosoftGraphAuthenticationConditions>] [-Description <String>] [-DisplayName <String>]
 [-Id <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Update
```
Update-MgIdentityAuthenticationEventFlow -AuthenticationEventsFlowId <String>
 -BodyParameter <IMicrosoftGraphAuthenticationEventsFlow> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgIdentityAuthenticationEventFlow -InputObject <IIdentitySignInsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Conditions <IMicrosoftGraphAuthenticationConditions>] [-Description <String>] [-DisplayName <String>]
 [-Id <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgIdentityAuthenticationEventFlow -InputObject <IIdentitySignInsIdentity>
 -BodyParameter <IMicrosoftGraphAuthenticationEventsFlow> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of an authenticationEventsFlow object by ID.
You must specify the @odata.type property and the value of the authenticationEventsFlow object type to update.
The following derived subtypes are supported:- externalUsersSelfServiceSignupEventsFlow

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | EventListener.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | EventListener.ReadWrite.All,  |

## EXAMPLES
### Example 1: Update the display name of an external identities self-service sign-up user flow

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.externalUsersSelfServiceSignUpEventsFlow"
	displayName = "New user flow description"
}

Update-MgIdentityAuthenticationEventFlow -AuthenticationEventsFlowId $authenticationEventsFlowId -BodyParameter $params

```
This example will update the display name of an external identities self-service sign-up user flow

### Example 2: Update the page layout of a self-service sign up user flow

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.externalUsersSelfServiceSignUpEventsFlow"
	onAttributeCollection = @{
		"@odata.type" = "#microsoft.graph.onAttributeCollectionExternalUsersSelfServiceSignUp"
		attributeCollectionPage = @{
			views = @(
				@{
					title = $null
					description = $null
					inputs = @(
						@{
							attribute = "email"
							label = "Email Address"
							inputType = "text"
							defaultValue = $null
							hidden = $true
							editable = $false
							writeToDirectory = $true
							required = $true
							validationRegEx = "^[a-zA-Z0-9.!#$%&amp;&#8217;'*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:.[a-zA-Z0-9-]+)*$"
							options = @(
							)
						}
						@{
							attribute = "displayName"
							label = "Display Name"
							inputType = "text"
							defaultValue = $null
							hidden = $false
							editable = $true
							writeToDirectory = $true
							required = $true
							validationRegEx = "^[a-zA-Z_][0-9a-zA-Z_ ]*[0-9a-zA-Z_]+$"
							options = @(
							)
						}
						@{
							attribute = "city"
							label = "City"
							inputType = "text"
							defaultValue = $null
							hidden = $false
							editable = $true
							writeToDirectory = $true
							required = $true
							validationRegEx = "^[a-zA-Z_][0-9a-zA-Z_ ]*[0-9a-zA-Z_]+$"
							options = @(
							)
						}
						@{
							attribute = "extension_331d514c0c18477583ea7dd5a79feda2_RockorCountry"
							label = "Rock music or Country"
							inputType = "radioSingleSelect"
							defaultValue = $null
							hidden = $false
							editable = $true
							writeToDirectory = $true
							required = $true
							validationRegEx = "^.*"
							options = @(
								@{
									label = "Rock music"
									value = "Rock"
								}
								@{
									label = "Country music"
									value = "Country"
								}
							)
						}
					)
				}
			)
		}
	}
}

Update-MgIdentityAuthenticationEventFlow -AuthenticationEventsFlowId $authenticationEventsFlowId -BodyParameter $params

```
This example will update the page layout of a self-service sign up user flow


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AuthenticationEventsFlowId
The unique identifier of authenticationEventsFlow

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
authenticationEventsFlow
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationEventsFlow
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Conditions
authenticationConditions
To construct, see NOTES section for CONDITIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationConditions
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### -Description
The description of the events policy.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Required.
The display name for the events policy.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IIdentitySignInsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### Microsoft.Graph.PowerShell.Models.IIdentitySignInsIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuthenticationEventsFlow
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuthenticationEventsFlow
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphAuthenticationEventsFlow>`: authenticationEventsFlow
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Conditions <IMicrosoftGraphAuthenticationConditions>]`: authenticationConditions
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Applications <IMicrosoftGraphAuthenticationConditionsApplications>]`: authenticationConditionsApplications
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IncludeApplications <IMicrosoftGraphAuthenticationConditionApplication- `[]`>]`:
        - `[AppId <String>]`: The identifier for an application corresponding to a condition which will trigger an authenticationEventListener.
  - `[Description <String>]`: The description of the events policy.
  - `[DisplayName <String>]`: Required.
The display name for the events policy.

CONDITIONS `<IMicrosoftGraphAuthenticationConditions>`: authenticationConditions
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Applications <IMicrosoftGraphAuthenticationConditionsApplications>]`: authenticationConditionsApplications
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IncludeApplications <IMicrosoftGraphAuthenticationConditionApplication- `[]`>]`:
      - `[AppId <String>]`: The identifier for an application corresponding to a condition which will trigger an authenticationEventListener.

INPUTOBJECT `<IIdentitySignInsIdentity>`: Identity Parameter
  - `[ActivityBasedTimeoutPolicyId <String>]`: The unique identifier of activityBasedTimeoutPolicy
  - `[AppManagementPolicyId <String>]`: The unique identifier of appManagementPolicy
  - `[AuthenticationCombinationConfigurationId <String>]`: The unique identifier of authenticationCombinationConfiguration
  - `[AuthenticationConditionApplicationAppId <String>]`: The unique identifier of authenticationConditionApplication
  - `[AuthenticationContextClassReferenceId <String>]`: The unique identifier of authenticationContextClassReference
  - `[AuthenticationEventListenerId <String>]`: The unique identifier of authenticationEventListener
  - `[AuthenticationEventsFlowId <String>]`: The unique identifier of authenticationEventsFlow
  - `[AuthenticationMethodConfigurationId <String>]`: The unique identifier of authenticationMethodConfiguration
  - `[AuthenticationMethodId <String>]`: The unique identifier of authenticationMethod
  - `[AuthenticationMethodModeDetailId <String>]`: The unique identifier of authenticationMethodModeDetail
  - `[AuthenticationStrengthPolicyId <String>]`: The unique identifier of authenticationStrengthPolicy
  - `[B2XIdentityUserFlowId <String>]`: The unique identifier of b2xIdentityUserFlow
  - `[BitlockerRecoveryKeyId <String>]`: The unique identifier of bitlockerRecoveryKey
  - `[CertificateBasedAuthConfigurationId <String>]`: The unique identifier of certificateBasedAuthConfiguration
  - `[ClaimsMappingPolicyId <String>]`: The unique identifier of claimsMappingPolicy
  - `[ConditionalAccessPolicyId <String>]`: The unique identifier of conditionalAccessPolicy
  - `[ConditionalAccessTemplateId <String>]`: The unique identifier of conditionalAccessTemplate
  - `[CrossTenantAccessPolicyConfigurationPartnerTenantId <String>]`: The unique identifier of crossTenantAccessPolicyConfigurationPartner
  - `[CustomAuthenticationExtensionId <String>]`: The unique identifier of customAuthenticationExtension
  - `[DataPolicyOperationId <String>]`: The unique identifier of dataPolicyOperation
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EmailAuthenticationMethodId <String>]`: The unique identifier of emailAuthenticationMethod
  - `[FeatureRolloutPolicyId <String>]`: The unique identifier of featureRolloutPolicy
  - `[Fido2AuthenticationMethodId <String>]`: The unique identifier of fido2AuthenticationMethod
  - `[HomeRealmDiscoveryPolicyId <String>]`: The unique identifier of homeRealmDiscoveryPolicy
  - `[IdentityApiConnectorId <String>]`: The unique identifier of identityApiConnector
  - `[IdentityProviderBaseId <String>]`: The unique identifier of identityProviderBase
  - `[IdentityProviderId <String>]`: The unique identifier of identityProvider
  - `[IdentityUserFlowAttributeAssignmentId <String>]`: The unique identifier of identityUserFlowAttributeAssignment
  - `[IdentityUserFlowAttributeId <String>]`: The unique identifier of identityUserFlowAttribute
  - `[LongRunningOperationId <String>]`: The unique identifier of longRunningOperation
  - `[MicrosoftAuthenticatorAuthenticationMethodId <String>]`: The unique identifier of microsoftAuthenticatorAuthenticationMethod
  - `[MultiTenantOrganizationMemberId <String>]`: The unique identifier of multiTenantOrganizationMember
  - `[NamedLocationId <String>]`: The unique identifier of namedLocation
  - `[OAuth2PermissionGrantId <String>]`: The unique identifier of oAuth2PermissionGrant
  - `[OrganizationId <String>]`: The unique identifier of organization
  - `[PasswordAuthenticationMethodId <String>]`: The unique identifier of passwordAuthenticationMethod
  - `[PermissionGrantConditionSetId <String>]`: The unique identifier of permissionGrantConditionSet
  - `[PermissionGrantPolicyId <String>]`: The unique identifier of permissionGrantPolicy
  - `[PhoneAuthenticationMethodId <String>]`: The unique identifier of phoneAuthenticationMethod
  - `[RiskDetectionId <String>]`: The unique identifier of riskDetection
  - `[RiskyServicePrincipalHistoryItemId <String>]`: The unique identifier of riskyServicePrincipalHistoryItem
  - `[RiskyServicePrincipalId <String>]`: The unique identifier of riskyServicePrincipal
  - `[RiskyUserHistoryItemId <String>]`: The unique identifier of riskyUserHistoryItem
  - `[RiskyUserId <String>]`: The unique identifier of riskyUser
  - `[ServicePrincipalRiskDetectionId <String>]`: The unique identifier of servicePrincipalRiskDetection
  - `[SoftwareOathAuthenticationMethodId <String>]`: The unique identifier of softwareOathAuthenticationMethod
  - `[TemporaryAccessPassAuthenticationMethodId <String>]`: The unique identifier of temporaryAccessPassAuthenticationMethod
  - `[ThreatAssessmentRequestId <String>]`: The unique identifier of threatAssessmentRequest
  - `[ThreatAssessmentResultId <String>]`: The unique identifier of threatAssessmentResult
  - `[TokenIssuancePolicyId <String>]`: The unique identifier of tokenIssuancePolicy
  - `[TokenLifetimePolicyId <String>]`: The unique identifier of tokenLifetimePolicy
  - `[UnifiedRoleManagementPolicyAssignmentId <String>]`: The unique identifier of unifiedRoleManagementPolicyAssignment
  - `[UnifiedRoleManagementPolicyId <String>]`: The unique identifier of unifiedRoleManagementPolicy
  - `[UnifiedRoleManagementPolicyRuleId <String>]`: The unique identifier of unifiedRoleManagementPolicyRule
  - `[UserFlowLanguageConfigurationId <String>]`: The unique identifier of userFlowLanguageConfiguration
  - `[UserFlowLanguagePageId <String>]`: The unique identifier of userFlowLanguagePage
  - `[UserId <String>]`: The unique identifier of user
  - `[WindowsHelloForBusinessAuthenticationMethodId <String>]`: The unique identifier of windowsHelloForBusinessAuthenticationMethod

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgidentityauthenticationeventflow](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgidentityauthenticationeventflow)

[https://learn.microsoft.com/graph/api/authenticationeventsflow-update?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/authenticationeventsflow-update?view=graph-rest-1.0)























