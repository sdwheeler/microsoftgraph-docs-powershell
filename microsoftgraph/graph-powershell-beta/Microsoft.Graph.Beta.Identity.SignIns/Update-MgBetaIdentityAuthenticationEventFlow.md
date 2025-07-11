---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaidentityauthenticationeventflow
schema: 2.0.0
ms.subservice: entra-sign-in
---

# Update-MgBetaIdentityAuthenticationEventFlow

## SYNOPSIS
Update the properties of an authenticationEventsFlow object by ID.
You must specify the @odata.type property and the value of the authenticationEventsFlow object type to update.
The following derived subtypes are supported:- externalUsersSelfServiceSignupEventsFlow

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgIdentityAuthenticationEventFlow](/powershell/module/Microsoft.Graph.Identity.SignIns/Update-MgIdentityAuthenticationEventFlow?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaIdentityAuthenticationEventFlow -AuthenticationEventsFlowId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Conditions <IMicrosoftGraphAuthenticationConditions>] [-Description <String>] [-DisplayName <String>]
 [-Id <String>] [-Priority <Int32>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaIdentityAuthenticationEventFlow -AuthenticationEventsFlowId <String>
 -BodyParameter <IMicrosoftGraphAuthenticationEventsFlow> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaIdentityAuthenticationEventFlow -InputObject <IIdentitySignInsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Conditions <IMicrosoftGraphAuthenticationConditions>] [-Description <String>] [-DisplayName <String>]
 [-Id <String>] [-Priority <Int32>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaIdentityAuthenticationEventFlow -InputObject <IIdentitySignInsIdentity>
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
### Example 1: Update the display name and priority of an authenticationEventsFlow

```powershell

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.externalUsersSelfServiceSignUpEventsFlow"
	displayName = "New user flow description"
	priority = 200
}

Update-MgBetaIdentityAuthenticationEventFlow -AuthenticationEventsFlowId $authenticationEventsFlowId -BodyParameter $params

```
This example will update the display name and priority of an authenticationeventsflow

### Example 2: Update the onAttributeCollection event of a self-service sign up user flow

```powershell

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.externalUsersSelfServiceSignUpEventsFlow"
	onAttributeCollection = @{
		"@odata.type" = "#microsoft.graph.onAttributeCollectionExternalUsersSelfServiceSignUp"
		attributeCollectionPage = @{
			customStringsFileId = $null
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
							required = $false
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
							required = $false
							validationRegEx = "^[a-zA-Z_][0-9a-zA-Z_ ]*[0-9a-zA-Z_]+$"
							options = @(
							)
						}
						@{
							attribute = "extension_6ea3bc85aec24b1c92ff4a117afb6621_Favoritecolor"
							label = "Favorite color"
							inputType = "text"
							defaultValue = $null
							hidden = $false
							editable = $true
							writeToDirectory = $true
							required = $false
							validationRegEx = "^.*"
							options = @(
							)
						}
					)
				}
			)
		}
	}
}

Update-MgBetaIdentityAuthenticationEventFlow -AuthenticationEventsFlowId $authenticationEventsFlowId -BodyParameter $params

```
This example will update the onattributecollection event of a self-service sign up user flow

### Example 3: Remove an attribute collected during a self-service sign up user flow

```powershell

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.externalUsersSelfServiceSignUpEventsFlow"
	onAttributeCollection = @{
		"@odata.type" = "#microsoft.graph.onAttributeCollectionExternalUsersSelfServiceSignUp"
		attributeCollectionPage = @{
			customStringsFileId = $null
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
							required = $false
							validationRegEx = "^[a-zA-Z_][0-9a-zA-Z_ ]*[0-9a-zA-Z_]+$"
							options = @(
							)
						}
						@{
							attribute = "extension_6ea3bc85aec24b1c92ff4a117afb6621_Favoritecolor"
							label = "Favorite color"
							inputType = "text"
							defaultValue = $null
							hidden = $false
							editable = $true
							writeToDirectory = $true
							required = $false
							validationRegEx = "^.*"
							options = @(
							)
						}
					)
				}
			)
		}
	}
}

Update-MgBetaIdentityAuthenticationEventFlow -AuthenticationEventsFlowId $authenticationEventsFlowId -BodyParameter $params

```
This example will remove an attribute collected during a self-service sign up user flow


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

### -Priority
The priority to use for each individual event of the events policy.
If multiple competing listeners for an event have the same priority, one is chosen and an error is silently logged.
Defaults to 500.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
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

### Microsoft.Graph.Beta.PowerShell.Models.IIdentitySignInsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAuthenticationEventsFlow
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAuthenticationEventsFlow
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
      - `[IncludeAllApplications <Boolean?>]`: Whether the custom authentication extension should trigger for all applications with appIds specified in the includeApplications relationship.
This property must be set to false for listener of type onTokenIssuanceStartListener.
      - `[IncludeApplications <IMicrosoftGraphAuthenticationConditionApplication- `[]`>]`: 
        - `[AppId <String>]`: The identifier for an application corresponding to a condition which will trigger an authenticationEventListener.
  - `[Description <String>]`: The description of the events policy.
  - `[DisplayName <String>]`: Required.
The display name for the events policy.
  - `[Priority <Int32?>]`: The priority to use for each individual event of the events policy.
If multiple competing listeners for an event have the same priority, one is chosen and an error is silently logged.
Defaults to 500.

CONDITIONS `<IMicrosoftGraphAuthenticationConditions>`: authenticationConditions
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Applications <IMicrosoftGraphAuthenticationConditionsApplications>]`: authenticationConditionsApplications
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IncludeAllApplications <Boolean?>]`: Whether the custom authentication extension should trigger for all applications with appIds specified in the includeApplications relationship.
This property must be set to false for listener of type onTokenIssuanceStartListener.
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
  - `[AuthenticationMethodModes <String- `[]`>]`: Usage: authenticationMethodModes={authenticationMethodModes}
  - `[AuthenticationStrengthPolicyId <String>]`: The unique identifier of authenticationStrengthPolicy
  - `[AuthorizationPolicyId <String>]`: The unique identifier of authorizationPolicy
  - `[B2CIdentityUserFlowId <String>]`: The unique identifier of b2cIdentityUserFlow
  - `[B2XIdentityUserFlowId <String>]`: The unique identifier of b2xIdentityUserFlow
  - `[BitlockerRecoveryKeyId <String>]`: The unique identifier of bitlockerRecoveryKey
  - `[CertificateBasedAuthConfigurationId <String>]`: The unique identifier of certificateBasedAuthConfiguration
  - `[ChangeItemBaseId <String>]`: The unique identifier of changeItemBase
  - `[ClaimsMappingPolicyId <String>]`: The unique identifier of claimsMappingPolicy
  - `[ConditionalAccessPolicyId <String>]`: The unique identifier of conditionalAccessPolicy
  - `[ConditionalAccessTemplateId <String>]`: The unique identifier of conditionalAccessTemplate
  - `[CrossTenantAccessPolicyConfigurationPartnerTenantId <String>]`: The unique identifier of crossTenantAccessPolicyConfigurationPartner
  - `[CustomAuthenticationExtensionId <String>]`: The unique identifier of customAuthenticationExtension
  - `[DataLossPreventionPolicyId <String>]`: The unique identifier of dataLossPreventionPolicy
  - `[DataPolicyOperationId <String>]`: The unique identifier of dataPolicyOperation
  - `[DefaultUserRoleOverrideId <String>]`: The unique identifier of defaultUserRoleOverride
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EmailAuthenticationMethodId <String>]`: The unique identifier of emailAuthenticationMethod
  - `[FeatureRolloutPolicyId <String>]`: The unique identifier of featureRolloutPolicy
  - `[Fido2AuthenticationMethodId <String>]`: The unique identifier of fido2AuthenticationMethod
  - `[GroupId <String>]`: The unique identifier of group
  - `[HardwareOathAuthenticationMethodId <String>]`: The unique identifier of hardwareOathAuthenticationMethod
  - `[HardwareOathTokenAuthenticationMethodDeviceId <String>]`: The unique identifier of hardwareOathTokenAuthenticationMethodDevice
  - `[HomeRealmDiscoveryPolicyId <String>]`: The unique identifier of homeRealmDiscoveryPolicy
  - `[IdentityApiConnectorId <String>]`: The unique identifier of identityApiConnector
  - `[IdentityProviderBaseId <String>]`: The unique identifier of identityProviderBase
  - `[IdentityProviderId <String>]`: The unique identifier of identityProvider
  - `[IdentityUserFlowAttributeAssignmentId <String>]`: The unique identifier of identityUserFlowAttributeAssignment
  - `[IdentityUserFlowAttributeId <String>]`: The unique identifier of identityUserFlowAttribute
  - `[IdentityUserFlowId <String>]`: The unique identifier of identityUserFlow
  - `[InformationProtectionLabelId <String>]`: The unique identifier of informationProtectionLabel
  - `[LongRunningOperationId <String>]`: The unique identifier of longRunningOperation
  - `[MicrosoftAuthenticatorAuthenticationMethodId <String>]`: The unique identifier of microsoftAuthenticatorAuthenticationMethod
  - `[MobilityManagementPolicyId <String>]`: The unique identifier of mobilityManagementPolicy
  - `[MultiTenantOrganizationMemberId <String>]`: The unique identifier of multiTenantOrganizationMember
  - `[NamedLocationId <String>]`: The unique identifier of namedLocation
  - `[OAuth2PermissionGrantId <String>]`: The unique identifier of oAuth2PermissionGrant
  - `[OrganizationId <String>]`: The unique identifier of organization
  - `[PasswordAuthenticationMethodId <String>]`: The unique identifier of passwordAuthenticationMethod
  - `[PasswordlessMicrosoftAuthenticatorAuthenticationMethodId <String>]`: The unique identifier of passwordlessMicrosoftAuthenticatorAuthenticationMethod
  - `[PermissionGrantConditionSetId <String>]`: The unique identifier of permissionGrantConditionSet
  - `[PermissionGrantPolicyId <String>]`: The unique identifier of permissionGrantPolicy
  - `[PermissionGrantPreApprovalPolicyId <String>]`: The unique identifier of permissionGrantPreApprovalPolicy
  - `[PhoneAuthenticationMethodId <String>]`: The unique identifier of phoneAuthenticationMethod
  - `[PlatformCredentialAuthenticationMethodId <String>]`: The unique identifier of platformCredentialAuthenticationMethod
  - `[RiskDetectionId <String>]`: The unique identifier of riskDetection
  - `[RiskyServicePrincipalHistoryItemId <String>]`: The unique identifier of riskyServicePrincipalHistoryItem
  - `[RiskyServicePrincipalId <String>]`: The unique identifier of riskyServicePrincipal
  - `[RiskyUserHistoryItemId <String>]`: The unique identifier of riskyUserHistoryItem
  - `[RiskyUserId <String>]`: The unique identifier of riskyUser
  - `[SensitivityLabelId <String>]`: The unique identifier of sensitivityLabel
  - `[SensitivityLabelId1 <String>]`: The unique identifier of sensitivityLabel
  - `[ServicePrincipalCreationConditionSetId <String>]`: The unique identifier of servicePrincipalCreationConditionSet
  - `[ServicePrincipalCreationPolicyId <String>]`: The unique identifier of servicePrincipalCreationPolicy
  - `[ServicePrincipalRiskDetectionId <String>]`: The unique identifier of servicePrincipalRiskDetection
  - `[SoftwareOathAuthenticationMethodId <String>]`: The unique identifier of softwareOathAuthenticationMethod
  - `[TemporaryAccessPassAuthenticationMethodId <String>]`: The unique identifier of temporaryAccessPassAuthenticationMethod
  - `[ThreatAssessmentRequestId <String>]`: The unique identifier of threatAssessmentRequest
  - `[ThreatAssessmentResultId <String>]`: The unique identifier of threatAssessmentResult
  - `[TokenIssuancePolicyId <String>]`: The unique identifier of tokenIssuancePolicy
  - `[TokenLifetimePolicyId <String>]`: The unique identifier of tokenLifetimePolicy
  - `[TrustFrameworkKeySetId <String>]`: The unique identifier of trustFrameworkKeySet
  - `[TrustFrameworkKeyV2Kid <String>]`: The unique identifier of trustFrameworkKey_v2
  - `[TrustFrameworkPolicyId <String>]`: The unique identifier of trustFrameworkPolicy
  - `[UnifiedRoleManagementPolicyAssignmentId <String>]`: The unique identifier of unifiedRoleManagementPolicyAssignment
  - `[UnifiedRoleManagementPolicyId <String>]`: The unique identifier of unifiedRoleManagementPolicy
  - `[UnifiedRoleManagementPolicyRuleId <String>]`: The unique identifier of unifiedRoleManagementPolicyRule
  - `[UserFlowLanguageConfigurationId <String>]`: The unique identifier of userFlowLanguageConfiguration
  - `[UserFlowLanguagePageId <String>]`: The unique identifier of userFlowLanguagePage
  - `[UserId <String>]`: The unique identifier of user
  - `[WindowsHelloForBusinessAuthenticationMethodId <String>]`: The unique identifier of windowsHelloForBusinessAuthenticationMethod

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaidentityauthenticationeventflow](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaidentityauthenticationeventflow)

[https://learn.microsoft.com/graph/api/authenticationeventsflow-update?view=graph-rest-beta](https://learn.microsoft.com/graph/api/authenticationeventsflow-update?view=graph-rest-beta)























