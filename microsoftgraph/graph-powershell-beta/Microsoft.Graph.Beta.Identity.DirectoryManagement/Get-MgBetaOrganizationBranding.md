---
external help file: Microsoft.Graph.Beta.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Beta.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/get-mgbetaorganizationbranding
schema: 2.0.0
ms.subservice: entra-sign-in
---

# Get-MgBetaOrganizationBranding

## SYNOPSIS
Retrieve the default organizational branding object, if the Accept-Language header is set to 0 or default.
If no default organizational branding object exists, this method returns a 404 Not Found error.
If the Accept-Language header is set to an existing locale identified by the value of its id, this method retrieves the branding for the specified locale.
This method retrieves only non-Stream properties, for example, usernameHintText and signInPageText.
To retrieve Stream types of the default branding, for example, bannerLogo and backgroundImage, use the GET organizationalBrandingLocalization method.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgOrganizationBranding](/powershell/module/Microsoft.Graph.Identity.DirectoryManagement/Get-MgOrganizationBranding?view=graph-powershell-1.0)

## SYNTAX

### Get (Default)
```
Get-MgBetaOrganizationBranding -OrganizationId <String> [-ExpandProperty <String[]>] [-Property <String[]>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaOrganizationBranding -InputObject <IIdentityDirectoryManagementIdentity> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Retrieve the default organizational branding object, if the Accept-Language header is set to 0 or default.
If no default organizational branding object exists, this method returns a 404 Not Found error.
If the Accept-Language header is set to an existing locale identified by the value of its id, this method retrieves the branding for the specified locale.
This method retrieves only non-Stream properties, for example, usernameHintText and signInPageText.
To retrieve Stream types of the default branding, for example, bannerLogo and backgroundImage, use the GET organizationalBrandingLocalization method.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | User.Read, User.Read.All, OrganizationalBranding.ReadWrite.All, OrganizationalBranding.Read.All, Organization.ReadWrite.All, Organization.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | OrganizationalBranding.Read.All, OrganizationalBranding.ReadWrite.All, Organization.ReadWrite.All, Organization.Read.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

Get-MgBetaOrganizationBranding -OrganizationId $organizationId

```
This example shows how to use the Get-MgBetaOrganizationBranding Cmdlet.

### Example 2: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

Get-MgBetaOrganizationBranding -OrganizationId $organizationId

```
This example shows how to use the Get-MgBetaOrganizationBranding Cmdlet.

### Example 3: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

Get-MgBetaOrganizationBranding -OrganizationId $organizationId

```
This example shows how to use the Get-MgBetaOrganizationBranding Cmdlet.


## PARAMETERS

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Expand

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IIdentityDirectoryManagementIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OrganizationId
The unique identifier of organization

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IIdentityDirectoryManagementIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphOrganizationalBranding
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/get-mgbetaorganizationbranding](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/get-mgbetaorganizationbranding)

[https://learn.microsoft.com/graph/api/organizationalbranding-get?view=graph-rest-beta](https://learn.microsoft.com/graph/api/organizationalbranding-get?view=graph-rest-beta)























