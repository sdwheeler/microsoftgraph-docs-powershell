---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/invoke-mgbetauploadtrustframeworkkeysetsecret
schema: 2.0.0
ms.subservice: entra-sign-in
---

# Invoke-MgBetaUploadTrustFrameworkKeySetSecret

## SYNOPSIS
Upload a plain text secret to a trustFrameworkKeyset.
Examples of secrets are application secrets in Microsoft Entra ID, Google, Facebook, or any other identity provider.
his method returns trustFrameworkKey.

## SYNTAX

### UploadExpanded (Default)
```
Invoke-MgBetaUploadTrustFrameworkKeySetSecret -TrustFrameworkKeySetId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Exp <Int64>] [-K <String>]
 [-Nbf <Int64>] [-Use <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Upload
```
Invoke-MgBetaUploadTrustFrameworkKeySetSecret -TrustFrameworkKeySetId <String>
 -BodyParameter <IPathsDmvqaiTrustframeworkKeysetsTrustframeworkkeysetIdMicrosoftGraphUploadsecretPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UploadViaIdentityExpanded
```
Invoke-MgBetaUploadTrustFrameworkKeySetSecret -InputObject <IIdentitySignInsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Exp <Int64>] [-K <String>]
 [-Nbf <Int64>] [-Use <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UploadViaIdentity
```
Invoke-MgBetaUploadTrustFrameworkKeySetSecret -InputObject <IIdentitySignInsIdentity>
 -BodyParameter <IPathsDmvqaiTrustframeworkKeysetsTrustframeworkkeysetIdMicrosoftGraphUploadsecretPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Upload a plain text secret to a trustFrameworkKeyset.
Examples of secrets are application secrets in Microsoft Entra ID, Google, Facebook, or any other identity provider.
his method returns trustFrameworkKey.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | TrustFrameworkKeySet.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | TrustFrameworkKeySet.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	use = "use-value"
	k = "application-secret-to-be-uploaded"
	nbf = 1508969811
	exp = 1508973711
}

Invoke-MgBetaUploadTrustFrameworkKeySetSecret -TrustFrameworkKeySetId $trustFrameworkKeySetId -BodyParameter $params

```
This example shows how to use the Invoke-MgBetaUploadTrustFrameworkKeySetSecret Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UploadExpanded, UploadViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter

To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPathsDmvqaiTrustframeworkKeysetsTrustframeworkkeysetIdMicrosoftGraphUploadsecretPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Upload, UploadViaIdentity
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

### -Exp


```yaml
Type: Int64
Parameter Sets: UploadExpanded, UploadViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IIdentitySignInsIdentity
Parameter Sets: UploadViaIdentityExpanded, UploadViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -K


```yaml
Type: String
Parameter Sets: UploadExpanded, UploadViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Nbf


```yaml
Type: Int64
Parameter Sets: UploadExpanded, UploadViaIdentityExpanded
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

### -TrustFrameworkKeySetId
The unique identifier of trustFrameworkKeySet

```yaml
Type: String
Parameter Sets: UploadExpanded, Upload
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Use


```yaml
Type: String
Parameter Sets: UploadExpanded, UploadViaIdentityExpanded
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
### Microsoft.Graph.Beta.PowerShell.Models.IPathsDmvqaiTrustframeworkKeysetsTrustframeworkkeysetIdMicrosoftGraphUploadsecretPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphTrustFrameworkKey
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsDmvqaiTrustframeworkKeysetsTrustframeworkkeysetIdMicrosoftGraphUploadsecretPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Exp <Int64?>]`: 
  - `[K <String>]`: 
  - `[Nbf <Int64?>]`: 
  - `[Use <String>]`: 

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/invoke-mgbetauploadtrustframeworkkeysetsecret](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/invoke-mgbetauploadtrustframeworkkeysetsecret)

[https://learn.microsoft.com/graph/api/trustframeworkkeyset-uploadsecret?view=graph-rest-beta](https://learn.microsoft.com/graph/api/trustframeworkkeyset-uploadsecret?view=graph-rest-beta)























