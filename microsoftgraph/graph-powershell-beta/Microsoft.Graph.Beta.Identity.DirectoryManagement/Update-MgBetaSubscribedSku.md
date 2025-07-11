---
external help file: Microsoft.Graph.Beta.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Beta.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/update-mgbetasubscribedsku
schema: 2.0.0
---

# Update-MgBetaSubscribedSku

## SYNOPSIS
Update entity in subscribedSkus

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgSubscribedSku](/powershell/module/Microsoft.Graph.Identity.DirectoryManagement/Update-MgSubscribedSku?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaSubscribedSku -SubscribedSkuId <String> [-ResponseHeadersVariable <String>] [-AccountId <String>]
 [-AccountName <String>] [-AdditionalProperties <Hashtable>] [-AppliesTo <String>] [-CapabilityStatus <String>]
 [-ConsumedUnits <Int32>] [-Id <String>] [-PrepaidUnits <IMicrosoftGraphLicenseUnitsDetail>]
 [-ServicePlans <IMicrosoftGraphServicePlanInfo[]>] [-SkuId <String>] [-SkuPartNumber <String>]
 [-SubscriptionIds <String[]>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaSubscribedSku -SubscribedSkuId <String> -BodyParameter <IMicrosoftGraphSubscribedSku>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaSubscribedSku -InputObject <IIdentityDirectoryManagementIdentity>
 [-ResponseHeadersVariable <String>] [-AccountId <String>] [-AccountName <String>]
 [-AdditionalProperties <Hashtable>] [-AppliesTo <String>] [-CapabilityStatus <String>]
 [-ConsumedUnits <Int32>] [-Id <String>] [-PrepaidUnits <IMicrosoftGraphLicenseUnitsDetail>]
 [-ServicePlans <IMicrosoftGraphServicePlanInfo[]>] [-SkuId <String>] [-SkuPartNumber <String>]
 [-SubscriptionIds <String[]>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaSubscribedSku -InputObject <IIdentityDirectoryManagementIdentity>
 -BodyParameter <IMicrosoftGraphSubscribedSku> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update entity in subscribedSkus

## EXAMPLES

## PARAMETERS

### -AccountId
The unique ID of the account this SKU belongs to.

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

### -AccountName
The name of the account this SKU belongs to.

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

### -AppliesTo
The target class for this SKU.
Only SKUs with target class User are assignable.
Possible values are: User, Company.

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
subscribedSku
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSubscribedSku
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CapabilityStatus
Enabled indicates that the prepaidUnits property has at least one unit that is enabled.
LockedOut indicates that the customer canceled their subscription.
Possible values are: Enabled, Warning, Suspended, Deleted, LockedOut.

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

### -ConsumedUnits
The number of licenses that have been assigned.

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
Type: IIdentityDirectoryManagementIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PrepaidUnits
licenseUnitsDetail
To construct, see NOTES section for PREPAIDUNITS properties and create a hash table.

```yaml
Type: IMicrosoftGraphLicenseUnitsDetail
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

### -ServicePlans
Information about the service plans that are available with the SKU.
Not nullable
To construct, see NOTES section for SERVICEPLANS properties and create a hash table.

```yaml
Type: IMicrosoftGraphServicePlanInfo[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SkuId
The unique identifier (GUID) for the service SKU.

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

### -SkuPartNumber
The SKU part number; for example, AAD_PREMIUM or RMSBASIC.
To get a list of commercial subscriptions that an organization has acquired, see List subscribedSkus.

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

### -SubscribedSkuId
The unique identifier of subscribedSku

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

### -SubscriptionIds
A list of all subscription IDs associated with this SKU.

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

### Microsoft.Graph.Beta.PowerShell.Models.IIdentityDirectoryManagementIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSubscribedSku
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSubscribedSku
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphSubscribedSku>`: subscribedSku
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AccountId <String>]`: The unique ID of the account this SKU belongs to.
  - `[AccountName <String>]`: The name of the account this SKU belongs to.
  - `[AppliesTo <String>]`: The target class for this SKU.
Only SKUs with target class User are assignable.
Possible values are: User, Company.
  - `[CapabilityStatus <String>]`: Enabled indicates that the prepaidUnits property has at least one unit that is enabled.
LockedOut indicates that the customer canceled their subscription.
Possible values are: Enabled, Warning, Suspended, Deleted, LockedOut.
  - `[ConsumedUnits <Int32?>]`: The number of licenses that have been assigned.
  - `[PrepaidUnits <IMicrosoftGraphLicenseUnitsDetail>]`: licenseUnitsDetail
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Enabled <Int32?>]`: The number of units that are enabled for the active subscription of the service SKU.
    - `[LockedOut <Int32?>]`: The number of units that are locked out because the customer canceled their subscription of the service SKU.
    - `[Suspended <Int32?>]`: The number of units that are suspended because the subscription of the service SKU has been canceled.
The units can't be assigned but can still be reactivated before they're deleted.
    - `[Warning <Int32?>]`: The number of units that are in warning status.
When the subscription of the service SKU has expired, the customer has a grace period to renew their subscription before it's canceled (moved to a suspended state).
  - `[ServicePlans <IMicrosoftGraphServicePlanInfo- `[]`>]`: Information about the service plans that are available with the SKU.
Not nullable
    - `[AppliesTo <String>]`: The object the service plan can be assigned to.
The possible values are: User - service plan can be assigned to individual users.Company - service plan can be assigned to the entire tenant.
    - `[ProvisioningStatus <String>]`: The provisioning status of the service plan.
The possible values are:Success - Service is fully provisioned.Disabled - Service is disabled.Error - The service plan isn't provisioned and is in an error state.PendingInput - The service isn't provisioned and is awaiting service confirmation.PendingActivation - The service is provisioned but requires explicit activation by an administrator (for example, Intune_O365 service plan)PendingProvisioning - Microsoft has added a new service to the product SKU and it isn't activated in the tenant.
    - `[ServicePlanId <String>]`: The unique identifier of the service plan.
    - `[ServicePlanName <String>]`: The name of the service plan.
  - `[SkuId <String>]`: The unique identifier (GUID) for the service SKU.
  - `[SkuPartNumber <String>]`: The SKU part number; for example, AAD_PREMIUM or RMSBASIC.
To get a list of commercial subscriptions that an organization has acquired, see List subscribedSkus.
  - `[SubscriptionIds <String- `[]`>]`: A list of all subscription IDs associated with this SKU.

INPUTOBJECT `<IIdentityDirectoryManagementIdentity>`: Identity Parameter
  - `[AdministrativeUnitId <String>]`: The unique identifier of administrativeUnit
  - `[AllowedValueId <String>]`: The unique identifier of allowedValue
  - `[AttributeSetId <String>]`: The unique identifier of attributeSet
  - `[CertificateAuthorityAsEntityId <String>]`: The unique identifier of certificateAuthorityAsEntity
  - `[CertificateAuthorityDetailId <String>]`: The unique identifier of certificateAuthorityDetail
  - `[CertificateBasedApplicationConfigurationId <String>]`: The unique identifier of certificateBasedApplicationConfiguration
  - `[CertificateBasedAuthPkiId <String>]`: The unique identifier of certificateBasedAuthPki
  - `[CommandId <String>]`: The unique identifier of command
  - `[CommerceSubscriptionId <String>]`: Alternate key of companySubscription
  - `[CompanySubscriptionId <String>]`: The unique identifier of companySubscription
  - `[ContractId <String>]`: The unique identifier of contract
  - `[CustomSecurityAttributeDefinitionId <String>]`: The unique identifier of customSecurityAttributeDefinition
  - `[DeviceId <String>]`: The unique identifier of device
  - `[DeviceLocalCredentialInfoId <String>]`: The unique identifier of deviceLocalCredentialInfo
  - `[DeviceTemplateId <String>]`: The unique identifier of deviceTemplate
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[DirectoryRoleId <String>]`: The unique identifier of directoryRole
  - `[DirectoryRoleTemplateId <String>]`: The unique identifier of directoryRoleTemplate
  - `[DirectorySettingId <String>]`: The unique identifier of directorySetting
  - `[DirectorySettingTemplateId <String>]`: The unique identifier of directorySettingTemplate
  - `[DomainDnsRecordId <String>]`: The unique identifier of domainDnsRecord
  - `[DomainId <String>]`: The unique identifier of domain
  - `[DomainName <String>]`: Usage: domainName='{domainName}'
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[ExternalUserProfileId <String>]`: The unique identifier of externalUserProfile
  - `[FeatureRolloutPolicyId <String>]`: The unique identifier of featureRolloutPolicy
  - `[HardwareOathTokenAuthenticationMethodDeviceId <String>]`: The unique identifier of hardwareOathTokenAuthenticationMethodDevice
  - `[IdentityProviderBaseId <String>]`: The unique identifier of identityProviderBase
  - `[ImpactedResourceId <String>]`: The unique identifier of impactedResource
  - `[InboundSharedUserProfileUserId <String>]`: The unique identifier of inboundSharedUserProfile
  - `[InternalDomainFederationId <String>]`: The unique identifier of internalDomainFederation
  - `[MutualTlsOauthConfigurationId <String>]`: The unique identifier of mutualTlsOauthConfiguration
  - `[OcpSubscriptionId <String>]`: Alternate key of companySubscription
  - `[OnPremisesDirectorySynchronizationId <String>]`: The unique identifier of onPremisesDirectorySynchronization
  - `[OrgContactId <String>]`: The unique identifier of orgContact
  - `[OrganizationId <String>]`: The unique identifier of organization
  - `[OrganizationalBrandingLocalizationId <String>]`: The unique identifier of organizationalBrandingLocalization
  - `[OutboundSharedUserProfileUserId <String>]`: The unique identifier of outboundSharedUserProfile
  - `[PendingExternalUserProfileId <String>]`: The unique identifier of pendingExternalUserProfile
  - `[ProfileCardPropertyId <String>]`: The unique identifier of profileCardProperty
  - `[RecommendationId <String>]`: The unique identifier of recommendation
  - `[RoleTemplateId <String>]`: Alternate key of directoryRole
  - `[ScopedRoleMembershipId <String>]`: The unique identifier of scopedRoleMembership
  - `[SharedEmailDomainId <String>]`: The unique identifier of sharedEmailDomain
  - `[SharedEmailDomainInvitationId <String>]`: The unique identifier of sharedEmailDomainInvitation
  - `[SubscribedSkuId <String>]`: The unique identifier of subscribedSku
  - `[TenantId <String>]`: Usage: tenantId='{tenantId}'
  - `[TenantReferenceTenantId <String>]`: The unique identifier of tenantReference
  - `[UsageRightId <String>]`: The unique identifier of usageRight
  - `[UserId <String>]`: The unique identifier of user

PREPAIDUNITS `<IMicrosoftGraphLicenseUnitsDetail>`: licenseUnitsDetail
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Enabled <Int32?>]`: The number of units that are enabled for the active subscription of the service SKU.
  - `[LockedOut <Int32?>]`: The number of units that are locked out because the customer canceled their subscription of the service SKU.
  - `[Suspended <Int32?>]`: The number of units that are suspended because the subscription of the service SKU has been canceled.
The units can't be assigned but can still be reactivated before they're deleted.
  - `[Warning <Int32?>]`: The number of units that are in warning status.
When the subscription of the service SKU has expired, the customer has a grace period to renew their subscription before it's canceled (moved to a suspended state).

SERVICEPLANS `<IMicrosoftGraphServicePlanInfo- `[]`>`: Information about the service plans that are available with the SKU.
Not nullable
  - `[AppliesTo <String>]`: The object the service plan can be assigned to.
The possible values are: User - service plan can be assigned to individual users.Company - service plan can be assigned to the entire tenant.
  - `[ProvisioningStatus <String>]`: The provisioning status of the service plan.
The possible values are:Success - Service is fully provisioned.Disabled - Service is disabled.Error - The service plan isn't provisioned and is in an error state.PendingInput - The service isn't provisioned and is awaiting service confirmation.PendingActivation - The service is provisioned but requires explicit activation by an administrator (for example, Intune_O365 service plan)PendingProvisioning - Microsoft has added a new service to the product SKU and it isn't activated in the tenant.
  - `[ServicePlanId <String>]`: The unique identifier of the service plan.
  - `[ServicePlanName <String>]`: The name of the service plan.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/update-mgbetasubscribedsku](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/update-mgbetasubscribedsku)
























