---
external help file: Microsoft.Graph.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/get-mgdomainfederationconfiguration
schema: 2.0.0
ms.subservice: entra-sign-in
ms.subservice: entra-sign-in
---

# Get-MgDomainFederationConfiguration

## SYNOPSIS
Read the properties and relationships of an internalDomainFederation object.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaDomainFederationConfiguration](/powershell/module/Microsoft.Graph.Beta.Identity.DirectoryManagement/Get-MgBetaDomainFederationConfiguration?view=graph-powershell-beta)

## SYNTAX

### List (Default)
```
Get-MgDomainFederationConfiguration -DomainId <String> [-ExpandProperty <String[]>] [-Property <String[]>]
 [-Filter <String>] [-Search <String>] [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PageSize <Int32>] [-All]
 [-CountVariable <String>] [<CommonParameters>]
```

### Get
```
Get-MgDomainFederationConfiguration -DomainId <String> -InternalDomainFederationId <String>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgDomainFederationConfiguration -InputObject <IIdentityDirectoryManagementIdentity>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

## DESCRIPTION
Read the properties and relationships of an internalDomainFederation object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Domain.ReadWrite.All, Domain.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Domain.ReadWrite.All, Domain.Read.All,  |

## EXAMPLES
### Example 1: Get the federation settings for a federated domain

```powershell
Get-MgDomainFederationConfiguration -DomainId 'contoso.com' -InternalDomainFederationId '2a8ce608-bb34-473f-9e0f-f373ee4cbc5a' | Format-List

ActiveSignInUri                       : https://sts.deverett.info/adfs/services/trust/2005/usernamemixed
DisplayName                           : Contoso
FederatedIdpMfaBehavior               : rejectMfaByFederatedIdp
Id                                    : 2a8ce608-bb34-473f-9e0f-f373ee4cbc5a
IsSignedAuthenticationRequestRequired :
IssuerUri                             : http://contoso.com/adfs/services/trust/
MetadataExchangeUri                   : https://sts.contoso.com/adfs/services/trust/mex
NextSigningCertificate                : MIIC3jCCAcagAwIBAgIQEt0T0G5GPZ9
PassiveSignInUri                      : https://sts.contoso.com/adfs/ls/
PreferredAuthenticationProtocol       : wsFed
PromptLoginBehavior                   :
SignOutUri                            : https://sts.deverett.info/adfs/ls/
SigningCertificate                    : MIIC3jCCAcagAwIBAgIQFsO0R8deG4h
SigningCertificateUpdateStatus        : Microsoft.Graph.PowerShell.Models.MicrosoftGraphSigningCertificateUpdateStatus
AdditionalProperties                    : {[@odata.context, https://graph.microsoft.com/v1.0/$metadata#domains('contoso.com')/federationConfiguration/$entity]}
```

This examples retrieves the federation settings for the specified domain.

## PARAMETERS

### -All
List all pages.

```yaml
Type: SwitchParameter
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CountVariable
Specifies a count of the total number of items in a collection.
By default, this variable will be set in the global scope.

```yaml
Type: String
Parameter Sets: List
Aliases: CV

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DomainId
The unique identifier of domain

```yaml
Type: String
Parameter Sets: List, Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: List
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

### -InternalDomainFederationId
The unique identifier of internalDomainFederation

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

### -PageSize
Sets the page size of results.

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
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

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Skip
Skip the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sort
Order items by property values

```yaml
Type: String[]
Parameter Sets: List
Aliases: OrderBy

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Top
Show only the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases: Limit

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IIdentityDirectoryManagementIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphInternalDomainFederation
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IIdentityDirectoryManagementIdentity>`: Identity Parameter
  - `[AdministrativeUnitId <String>]`: The unique identifier of administrativeUnit
  - `[AllowedValueId <String>]`: The unique identifier of allowedValue
  - `[AttributeSetId <String>]`: The unique identifier of attributeSet
  - `[CommerceSubscriptionId <String>]`: Alternate key of companySubscription
  - `[CompanySubscriptionId <String>]`: The unique identifier of companySubscription
  - `[ContractId <String>]`: The unique identifier of contract
  - `[CustomSecurityAttributeDefinitionId <String>]`: The unique identifier of customSecurityAttributeDefinition
  - `[DeviceId <String>]`: The unique identifier of device
  - `[DeviceLocalCredentialInfoId <String>]`: The unique identifier of deviceLocalCredentialInfo
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[DirectoryRoleId <String>]`: The unique identifier of directoryRole
  - `[DirectoryRoleTemplateId <String>]`: The unique identifier of directoryRoleTemplate
  - `[DomainDnsRecordId <String>]`: The unique identifier of domainDnsRecord
  - `[DomainId <String>]`: The unique identifier of domain
  - `[DomainName <String>]`: Usage: domainName='{domainName}'
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[IdentityProviderBaseId <String>]`: The unique identifier of identityProviderBase
  - `[InternalDomainFederationId <String>]`: The unique identifier of internalDomainFederation
  - `[OnPremisesDirectorySynchronizationId <String>]`: The unique identifier of onPremisesDirectorySynchronization
  - `[OrgContactId <String>]`: The unique identifier of orgContact
  - `[OrganizationId <String>]`: The unique identifier of organization
  - `[OrganizationalBrandingLocalizationId <String>]`: The unique identifier of organizationalBrandingLocalization
  - `[ProfileCardPropertyId <String>]`: The unique identifier of profileCardProperty
  - `[RoleTemplateId <String>]`: Alternate key of directoryRole
  - `[ScopedRoleMembershipId <String>]`: The unique identifier of scopedRoleMembership
  - `[SubscribedSkuId <String>]`: The unique identifier of subscribedSku
  - `[TenantId <String>]`: Usage: tenantId='{tenantId}'
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/get-mgdomainfederationconfiguration](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/get-mgdomainfederationconfiguration)

[https://learn.microsoft.com/graph/api/internaldomainfederation-get?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/internaldomainfederation-get?view=graph-rest-1.0)

[https://learn.microsoft.com/graph/api/domain-list-federationconfiguration?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/domain-list-federationconfiguration?view=graph-rest-1.0)























