---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgpolicypermissiongrantpolicyinclude
schema: 2.0.0
ms.subservice: entra-sign-in
---

# New-MgPolicyPermissionGrantPolicyInclude

## SYNOPSIS
Add conditions under which a permission grant event is *included* in a permission grant policy.
You do this by adding a permissionGrantConditionSet to the includes collection of a  permissionGrantPolicy.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaPolicyPermissionGrantPolicyInclude](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/New-MgBetaPolicyPermissionGrantPolicyInclude?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgPolicyPermissionGrantPolicyInclude -PermissionGrantPolicyId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ClientApplicationIds <String[]>]
 [-ClientApplicationPublisherIds <String[]>] [-ClientApplicationTenantIds <String[]>]
 [-ClientApplicationsFromVerifiedPublisherOnly] [-Id <String>] [-PermissionClassification <String>]
 [-PermissionType <String>] [-Permissions <String[]>] [-ResourceApplication <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgPolicyPermissionGrantPolicyInclude -PermissionGrantPolicyId <String>
 -BodyParameter <IMicrosoftGraphPermissionGrantConditionSet> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgPolicyPermissionGrantPolicyInclude -InputObject <IIdentitySignInsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-ClientApplicationIds <String[]>]
 [-ClientApplicationPublisherIds <String[]>] [-ClientApplicationTenantIds <String[]>]
 [-ClientApplicationsFromVerifiedPublisherOnly] [-Id <String>] [-PermissionClassification <String>]
 [-PermissionType <String>] [-Permissions <String[]>] [-ResourceApplication <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgPolicyPermissionGrantPolicyInclude -InputObject <IIdentitySignInsIdentity>
 -BodyParameter <IMicrosoftGraphPermissionGrantConditionSet> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Add conditions under which a permission grant event is *included* in a permission grant policy.
You do this by adding a permissionGrantConditionSet to the includes collection of a  permissionGrantPolicy.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Policy.ReadWrite.PermissionGrant,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Policy.ReadWrite.PermissionGrant,  |

## EXAMPLES
### Example 1: Create a permission grant policy include

```powershell
Connect-MgGraph -Scopes "Policy.Read.PermissionGrant,Policy.ReadWrite.PermissionGrant"
New-MgPolicyPermissionGrantPolicyInclude -PermissionGrantPolicyId "testtenant-sampleapp-permissions" -PermissionType "application" -ResourceApplication "00000000-0000-0000-0000-000000000000" -Permissions "00000000-0000-0000-0000-000000000000"  | fl

ClientApplicationIds                        : {all}
ClientApplicationPublisherIds               : {all}
ClientApplicationTenantIds                  : {all}
ClientApplicationsFromVerifiedPublisherOnly : False
Id                                          : 084b9abc-cf56-4d84-bdb0-5ad8f3a51038
PermissionClassification                    : all
PermissionType                              : application
Permissions                                 : {00000000-0000-0000-0000-000000000000}
ResourceApplication                         : 00000000-0000-0000-0000-000000000000
AdditionalProperties                        : {[@odata.context, https://graph.microsoft.com/v1.0/$metadata#policies/permissionGrantPolicies('testtenant-sampleapp-permissions')/includes/$entity]}
```

This command creates a new permission grant policy include configuration for the specified permission grant policy in Azure AD.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ClientApplicationIds
A list of appId values for the client applications to match with, or a list with the single value all to match any client application.
Default is the single value all.

```yaml
Type: String[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientApplicationsFromVerifiedPublisherOnly
Set to true to only match on client applications with a verified publisher.
Set to false to match on any client app, even if it doesn't have a verified publisher.
Default is false.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PermissionClassification
The permission classification for the permission being granted, or all to match with any permission classification (including permissions that aren't classified).
Default is all.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PermissionGrantPolicyId
The unique identifier of permissionGrantPolicy

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Permissions
The list of id values for the specific permissions to match with, or a list with the single value all to match with any permission.
The id of delegated permissions can be found in the oauth2PermissionScopes property of the API's servicePrincipal object.
The id of application permissions can be found in the appRoles property of the API's servicePrincipal object.
The id of resource-specific application permissions can be found in the resourceSpecificApplicationPermissions property of the API's servicePrincipal object.
Default is the single value all.

```yaml
Type: String[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceApplication
The appId of the resource application (for example the API) for which a permission is being granted, or any to match with any resource application or API.
Default is any.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPermissionGrantConditionSet
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPermissionGrantConditionSet
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphPermissionGrantConditionSet>`: permissionGrantConditionSet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ClientApplicationIds <String- `[]`>]`: A list of appId values for the client applications to match with, or a list with the single value all to match any client application.
Default is the single value all.
  - `[ClientApplicationPublisherIds <String- `[]`>]`: A list of Microsoft Partner Network (MPN) IDs for verified publishers of the client application, or a list with the single value all to match with client apps from any publisher.
Default is the single value all.
  - `[ClientApplicationTenantIds <String- `[]`>]`: A list of Microsoft Entra tenant IDs in which the client application is registered, or a list with the single value all to match with client apps registered in any tenant.
Default is the single value all.
  - `[ClientApplicationsFromVerifiedPublisherOnly <Boolean?>]`: Set to true to only match on client applications with a verified publisher.
Set to false to match on any client app, even if it doesn't have a verified publisher.
Default is false.
  - `[PermissionClassification <String>]`: The permission classification for the permission being granted, or all to match with any permission classification (including permissions that aren't classified).
Default is all.
  - `[PermissionType <String>]`: permissionType
  - `[Permissions <String- `[]`>]`: The list of id values for the specific permissions to match with, or a list with the single value all to match with any permission.
The id of delegated permissions can be found in the oauth2PermissionScopes property of the API's servicePrincipal object.
The id of application permissions can be found in the appRoles property of the API's servicePrincipal object.
The id of resource-specific application permissions can be found in the resourceSpecificApplicationPermissions property of the API's servicePrincipal object.
Default is the single value all.
  - `[ResourceApplication <String>]`: The appId of the resource application (for example the API) for which a permission is being granted, or any to match with any resource application or API.
Default is any.

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgpolicypermissiongrantpolicyinclude](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgpolicypermissiongrantpolicyinclude)

[https://learn.microsoft.com/graph/api/permissiongrantpolicy-post-includes?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/permissiongrantpolicy-post-includes?view=graph-rest-1.0)























