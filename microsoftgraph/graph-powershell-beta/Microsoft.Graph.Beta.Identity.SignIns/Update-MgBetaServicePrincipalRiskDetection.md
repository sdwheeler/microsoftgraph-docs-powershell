---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaserviceprincipalriskdetection
schema: 2.0.0
---

# Update-MgBetaServicePrincipalRiskDetection

## SYNOPSIS
Update the navigation property servicePrincipalRiskDetections in identityProtection

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgServicePrincipalRiskDetection](/powershell/module/Microsoft.Graph.Identity.SignIns/Update-MgServicePrincipalRiskDetection?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaServicePrincipalRiskDetection -ServicePrincipalRiskDetectionId <String>
 [-ResponseHeadersVariable <String>] [-Activity <String>] [-ActivityDateTime <DateTime>]
 [-AdditionalInfo <String>] [-AdditionalProperties <Hashtable>] [-AppId <String>] [-CorrelationId <String>]
 [-DetectedDateTime <DateTime>] [-DetectionTimingType <String>] [-IPAddress <String>] [-Id <String>]
 [-KeyIds <String[]>] [-LastUpdatedDateTime <DateTime>] [-Location <IMicrosoftGraphSignInLocation>]
 [-MitreTechniqueId <String>] [-RequestId <String>] [-RiskDetail <String>] [-RiskEventType <String>]
 [-RiskLevel <String>] [-RiskState <String>] [-ServicePrincipalDisplayName <String>]
 [-ServicePrincipalId <String>] [-Source <String>] [-TokenIssuerType <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaServicePrincipalRiskDetection -ServicePrincipalRiskDetectionId <String>
 -BodyParameter <IMicrosoftGraphServicePrincipalRiskDetection> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaServicePrincipalRiskDetection -InputObject <IIdentitySignInsIdentity>
 [-ResponseHeadersVariable <String>] [-Activity <String>] [-ActivityDateTime <DateTime>]
 [-AdditionalInfo <String>] [-AdditionalProperties <Hashtable>] [-AppId <String>] [-CorrelationId <String>]
 [-DetectedDateTime <DateTime>] [-DetectionTimingType <String>] [-IPAddress <String>] [-Id <String>]
 [-KeyIds <String[]>] [-LastUpdatedDateTime <DateTime>] [-Location <IMicrosoftGraphSignInLocation>]
 [-MitreTechniqueId <String>] [-RequestId <String>] [-RiskDetail <String>] [-RiskEventType <String>]
 [-RiskLevel <String>] [-RiskState <String>] [-ServicePrincipalDisplayName <String>]
 [-ServicePrincipalId <String>] [-Source <String>] [-TokenIssuerType <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaServicePrincipalRiskDetection -InputObject <IIdentitySignInsIdentity>
 -BodyParameter <IMicrosoftGraphServicePrincipalRiskDetection> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property servicePrincipalRiskDetections in identityProtection

## EXAMPLES

## PARAMETERS

### -Activity
activityType

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

### -ActivityDateTime
Date and time when the risky activity occurred.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AdditionalInfo
Additional information associated with the risk detection.
This string value is represented as a JSON object with the quotations escaped.

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

### -AppId
The unique identifier for the associated application.

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

### -BodyParameter
servicePrincipalRiskDetection
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphServicePrincipalRiskDetection
Parameter Sets: Update, UpdateViaIdentity
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

### -CorrelationId
Correlation ID of the sign-in activity associated with the risk detection.
This property is null if the risk detection isn't associated with a sign-in activity.

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

### -DetectedDateTime
Date and time when the risk was detected.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DetectionTimingType
riskDetectionTimingType

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

### -IPAddress
Provides the IP address of the client from where the risk occurred.

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

### -KeyIds
The unique identifier (GUID) for the key credential associated with the risk detection.

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

### -LastUpdatedDateTime
Date and time when the risk detection was last updated.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Location
signInLocation
To construct, see NOTES section for LOCATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphSignInLocation
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MitreTechniqueId


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

### -RequestId
Request identifier of the sign-in activity associated with the risk detection.
This property is null if the risk detection isn't associated with a sign-in activity.
Supports $filter (eq).

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

### -RiskDetail
riskDetail

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

### -RiskEventType
The type of risk event detected.
The possible values are: investigationsThreatIntelligence, generic, adminConfirmedServicePrincipalCompromised, suspiciousSignins, leakedCredentials, anomalousServicePrincipalActivity, maliciousApplication, suspiciousApplication, suspiciousAPITraffic.

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

### -RiskLevel
riskLevel

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

### -RiskState
riskState

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

### -ServicePrincipalDisplayName
The display name for the service principal.

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

### -ServicePrincipalId
The unique identifier for the service principal.
Supports $filter (eq).

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

### -ServicePrincipalRiskDetectionId
The unique identifier of servicePrincipalRiskDetection

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

### -Source
Source of the risk detection.
For example, identityProtection.

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

### -TokenIssuerType
tokenIssuerType

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
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphServicePrincipalRiskDetection
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphServicePrincipalRiskDetection
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphServicePrincipalRiskDetection>`: servicePrincipalRiskDetection
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Activity <String>]`: activityType
  - `[ActivityDateTime <DateTime?>]`: Date and time when the risky activity occurred.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[AdditionalInfo <String>]`: Additional information associated with the risk detection.
This string value is represented as a JSON object with the quotations escaped.
  - `[AppId <String>]`: The unique identifier for the associated application.
  - `[CorrelationId <String>]`: Correlation ID of the sign-in activity associated with the risk detection.
This property is null if the risk detection isn't associated with a sign-in activity.
  - `[DetectedDateTime <DateTime?>]`: Date and time when the risk was detected.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[DetectionTimingType <String>]`: riskDetectionTimingType
  - `[IPAddress <String>]`: Provides the IP address of the client from where the risk occurred.
  - `[KeyIds <String- `[]`>]`: The unique identifier (GUID) for the key credential associated with the risk detection.
  - `[LastUpdatedDateTime <DateTime?>]`: Date and time when the risk detection was last updated.
  - `[Location <IMicrosoftGraphSignInLocation>]`: signInLocation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[City <String>]`: Provides the city where the sign-in originated.
This is calculated using latitude/longitude information from the sign-in activity.
    - `[CountryOrRegion <String>]`: Provides the country code info (two letter code) where the sign-in originated. 
This is calculated using latitude/longitude information from the sign-in activity.
    - `[GeoCoordinates <IMicrosoftGraphGeoCoordinates>]`: geoCoordinates
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Altitude <Double?>]`: Optional.
The altitude (height), in feet,  above sea level for the item.
Read-only.
      - `[Latitude <Double?>]`: Optional.
The latitude, in decimal, for the item.
Writable on OneDrive Personal.
      - `[Longitude <Double?>]`: Optional.
The longitude, in decimal, for the item.
Writable on OneDrive Personal.
    - `[State <String>]`: Provides the State where the sign-in originated.
This is calculated using latitude/longitude information from the sign-in activity.
  - `[MitreTechniqueId <String>]`: 
  - `[RequestId <String>]`: Request identifier of the sign-in activity associated with the risk detection.
This property is null if the risk detection isn't associated with a sign-in activity.
Supports $filter (eq).
  - `[RiskDetail <String>]`: riskDetail
  - `[RiskEventType <String>]`: The type of risk event detected.
The possible values are: investigationsThreatIntelligence, generic, adminConfirmedServicePrincipalCompromised, suspiciousSignins, leakedCredentials, anomalousServicePrincipalActivity, maliciousApplication, suspiciousApplication, suspiciousAPITraffic.
  - `[RiskLevel <String>]`: riskLevel
  - `[RiskState <String>]`: riskState
  - `[ServicePrincipalDisplayName <String>]`: The display name for the service principal.
  - `[ServicePrincipalId <String>]`: The unique identifier for the service principal.
Supports $filter (eq).
  - `[Source <String>]`: Source of the risk detection.
For example, identityProtection.
  - `[TokenIssuerType <String>]`: tokenIssuerType

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

LOCATION `<IMicrosoftGraphSignInLocation>`: signInLocation
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[City <String>]`: Provides the city where the sign-in originated.
This is calculated using latitude/longitude information from the sign-in activity.
  - `[CountryOrRegion <String>]`: Provides the country code info (two letter code) where the sign-in originated. 
This is calculated using latitude/longitude information from the sign-in activity.
  - `[GeoCoordinates <IMicrosoftGraphGeoCoordinates>]`: geoCoordinates
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Altitude <Double?>]`: Optional.
The altitude (height), in feet,  above sea level for the item.
Read-only.
    - `[Latitude <Double?>]`: Optional.
The latitude, in decimal, for the item.
Writable on OneDrive Personal.
    - `[Longitude <Double?>]`: Optional.
The longitude, in decimal, for the item.
Writable on OneDrive Personal.
  - `[State <String>]`: Provides the State where the sign-in originated.
This is calculated using latitude/longitude information from the sign-in activity.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaserviceprincipalriskdetection](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaserviceprincipalriskdetection)
























