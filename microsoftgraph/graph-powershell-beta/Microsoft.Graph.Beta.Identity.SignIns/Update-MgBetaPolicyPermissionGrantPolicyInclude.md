---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetapolicypermissiongrantpolicyinclude
schema: 2.0.0
---

# Update-MgBetaPolicyPermissionGrantPolicyInclude

## SYNOPSIS
Update the navigation property includes in policies

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgPolicyPermissionGrantPolicyInclude](/powershell/module/Microsoft.Graph.Identity.SignIns/Update-MgPolicyPermissionGrantPolicyInclude?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaPolicyPermissionGrantPolicyInclude -PermissionGrantConditionSetId <String>
 -PermissionGrantPolicyId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-CertifiedClientApplicationsOnly] [-ClientApplicationIds <String[]>]
 [-ClientApplicationPublisherIds <String[]>] [-ClientApplicationTenantIds <String[]>]
 [-ClientApplicationsFromVerifiedPublisherOnly] [-Id <String>] [-PermissionClassification <String>]
 [-PermissionType <String>] [-Permissions <String[]>] [-ResourceApplication <String>]
 [-ScopeSensitivityLabels <IMicrosoftGraphScopeSensitivityLabels>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaPolicyPermissionGrantPolicyInclude -PermissionGrantConditionSetId <String>
 -PermissionGrantPolicyId <String> -BodyParameter <IMicrosoftGraphPermissionGrantConditionSet>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaPolicyPermissionGrantPolicyInclude -InputObject <IIdentitySignInsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-CertifiedClientApplicationsOnly]
 [-ClientApplicationIds <String[]>] [-ClientApplicationPublisherIds <String[]>]
 [-ClientApplicationTenantIds <String[]>] [-ClientApplicationsFromVerifiedPublisherOnly] [-Id <String>]
 [-PermissionClassification <String>] [-PermissionType <String>] [-Permissions <String[]>]
 [-ResourceApplication <String>] [-ScopeSensitivityLabels <IMicrosoftGraphScopeSensitivityLabels>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaPolicyPermissionGrantPolicyInclude -InputObject <IIdentitySignInsIdentity>
 -BodyParameter <IMicrosoftGraphPermissionGrantConditionSet> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property includes in policies

## EXAMPLES
### Example 1: Update a permission grant policy include

```powershell
Connect-MgGraph -Scopes "Policy.Read.PermissionGrant,Policy.ReadWrite.PermissionGrant"  
Update-MgBetaPolicyPermissionGrantPolicyInclude -PermissionGrantConditionSetId "084b9abc-cf56-4d84-bdb0-5ad8f3a51038" -PermissionGrantPolicyId "testtenant-sampleapp-permissions" -PermissionType "application" -ResourceApplication "00000000-0000-0000-0000-000000000000" -Permissions "00000000-0000-0000-0000-000000000000", "00000000-0000-0000-0000-000000000001"
```

This command replaces the existing values with the provided new values for the specified include configuration properties in the specified permission grant policy in Azure AD.

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

### -BodyParameter
permissionGrantConditionSet
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPermissionGrantConditionSet
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CertifiedClientApplicationsOnly
Set to true to only match on client applications that are Microsoft 365 certified.
Set to false to match on any other client app.
Default is false.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientApplicationIds
A list of appId values for the client applications to match with, or a list with the single value all to match any client application.
Default is the single value all.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientApplicationPublisherIds
A list of Microsoft Partner Network (MPN) IDs for verified publishers of the client application, or a list with the single value all to match with client apps from any publisher.
Default is the single value all.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientApplicationsFromVerifiedPublisherOnly
Set to true to only match on client applications with a verified publisher.
Set to false to match on any client app, even if it does not have a verified publisher.
Default is false.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientApplicationTenantIds
A list of Microsoft Entra tenant IDs in which the client application is registered, or a list with the single value all to match with client apps registered in any tenant.
Default is the single value all.

```yaml
Type: String[]
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

### -PermissionClassification
The permission classification for the permission being granted, or all to match with any permission classification (including permissions which are not classified).
Default is all.

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

### -PermissionGrantConditionSetId
The unique identifier of permissionGrantConditionSet

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

### -PermissionGrantPolicyId
The unique identifier of permissionGrantPolicy

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

### -Permissions
The list of id values for the specific permissions to match with, or a list with the single value all to match with any permission.
The id of delegated permissions can be found in the publishedPermissionScopes property of the API's servicePrincipal object.
The id of application permissions can be found in the appRoles property of the API's servicePrincipal object.
The id of resource-specific application permissions can be found in the resourceSpecificApplicationPermissions property of the API's servicePrincipal object.
Default is the single value all.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PermissionType
permissionType

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

### -ResourceApplication
The appId of the resource application (e.g.
the API) for which a permission is being granted, or any to match with any resource application or API.
Default is any.

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

### -ScopeSensitivityLabels
scopeSensitivityLabels
To construct, see NOTES section for SCOPESENSITIVITYLABELS properties and create a hash table.

```yaml
Type: IMicrosoftGraphScopeSensitivityLabels
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

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
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPermissionGrantConditionSet
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPermissionGrantConditionSet
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphPermissionGrantConditionSet>`: permissionGrantConditionSet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CertifiedClientApplicationsOnly <Boolean?>]`: Set to true to only match on client applications that are Microsoft 365 certified.
Set to false to match on any other client app.
Default is false.
  - `[ClientApplicationIds <String- `[]`>]`: A list of appId values for the client applications to match with, or a list with the single value all to match any client application.
Default is the single value all.
  - `[ClientApplicationPublisherIds <String- `[]`>]`: A list of Microsoft Partner Network (MPN) IDs for verified publishers of the client application, or a list with the single value all to match with client apps from any publisher.
Default is the single value all.
  - `[ClientApplicationTenantIds <String- `[]`>]`: A list of Microsoft Entra tenant IDs in which the client application is registered, or a list with the single value all to match with client apps registered in any tenant.
Default is the single value all.
  - `[ClientApplicationsFromVerifiedPublisherOnly <Boolean?>]`: Set to true to only match on client applications with a verified publisher.
Set to false to match on any client app, even if it does not have a verified publisher.
Default is false.
  - `[PermissionClassification <String>]`: The permission classification for the permission being granted, or all to match with any permission classification (including permissions which are not classified).
Default is all.
  - `[PermissionType <String>]`: permissionType
  - `[Permissions <String- `[]`>]`: The list of id values for the specific permissions to match with, or a list with the single value all to match with any permission.
The id of delegated permissions can be found in the publishedPermissionScopes property of the API's servicePrincipal object.
The id of application permissions can be found in the appRoles property of the API's servicePrincipal object.
The id of resource-specific application permissions can be found in the resourceSpecificApplicationPermissions property of the API's servicePrincipal object.
Default is the single value all.
  - `[ResourceApplication <String>]`: The appId of the resource application (e.g.
the API) for which a permission is being granted, or any to match with any resource application or API.
Default is any.
  - `[ScopeSensitivityLabels <IMicrosoftGraphScopeSensitivityLabels>]`: scopeSensitivityLabels
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[LabelKind <String>]`: labelKind

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

SCOPESENSITIVITYLABELS `<IMicrosoftGraphScopeSensitivityLabels>`: scopeSensitivityLabels
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[LabelKind <String>]`: labelKind

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetapolicypermissiongrantpolicyinclude](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetapolicypermissiongrantpolicyinclude)























