---
external help file: Microsoft.Graph.Beta.Applications-help.xml
Module Name: Microsoft.Graph.Beta.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/get-mgbetaserviceprincipalapproleassignment
schema: 2.0.0
ms.subservice: entra-applications
ms.subservice: entra-applications
---

# Get-MgBetaServicePrincipalAppRoleAssignment

## SYNOPSIS
Read the properties and relationships of an appRoleAssignment object.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgServicePrincipalAppRoleAssignment](/powershell/module/Microsoft.Graph.Applications/Get-MgServicePrincipalAppRoleAssignment?view=graph-powershell-1.0)

## SYNTAX

### List (Default)
```
Get-MgBetaServicePrincipalAppRoleAssignment -ServicePrincipalId <String> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-Filter <String>] [-Search <String>] [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>]
 [-ConsistencyLevel <String>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PageSize <Int32>]
 [-All] [-CountVariable <String>] [<CommonParameters>]
```

### Get
```
Get-MgBetaServicePrincipalAppRoleAssignment -AppRoleAssignmentId <String> -ServicePrincipalId <String>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaServicePrincipalAppRoleAssignment -InputObject <IApplicationsIdentity> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Read the properties and relationships of an appRoleAssignment object.

## EXAMPLES
### Example 1: Get all application role assignments for a service principal

```powershell
Get-MgBetaServicePrincipalAppRoleAssignment -ServicePrincipalId '0bdb123d-b8a7-4cc9-8cc2-bd17bad06f61' |  Format-List

AppRoleId            : 00000000-0000-0000-0000-000000000000
CreatedDateTime      : 8/31/2021 2:01:28 PM
DeletedDateTime      :
Id                   : PRLbC6e4yUyMwr0XutBvYfZHkKGzlbxDr2I-QJWN9rs
PrincipalDisplayName : Example App
PrincipalId          : 0bdb123d-b8a7-4cc9-8cc2-bd17bad06f61
PrincipalType        : ServicePrincipal
ResourceDisplayName  : Office 365 Management APIs
ResourceId           : 557aedfc-007c-4904-918a-7e6fed2e7403
AdditionalProperties : {[@odata.id, https://graph.microsoft.com/v2/fb625e04-52aa-42da-b10d-14f1195d665f/directoryObjects/$/Microsof
                       t.DirectoryServices.ServicePrincipal('0bdb123d-b8a7-4cc9-8cc2-bd17bad06f61')/appRoleAssignments/PRLbC6e4yUyM
                       wr0XutBvYfZHkKGzlbxDr2I-QJWN9rs]}

AppRoleId            : 00000000-0000-0000-0000-000000000000
CreatedDateTime      : 8/31/2021 1:59:44 PM
DeletedDateTime      :
Id                   : PRLbC6e4yUyMwr0XutBvYZsr7FiAW3pIqP4F9944yBc
PrincipalDisplayName : Example App
PrincipalId          : 0bdb123d-b8a7-4cc9-8cc2-bd17bad06f61
PrincipalType        : ServicePrincipal
ResourceDisplayName  : Office 365 SharePoint Online
ResourceId           : 1c48f923-4fbb-4d37-b772-4d577eefec9e
AdditionalProperties : {[@odata.id, https://graph.microsoft.com/v2/fb625e04-52aa-42da-b10d-14f1195d665f/directoryObjects/$/Microsof
                       t.DirectoryServices.ServicePrincipal('0bdb123d-b8a7-4cc9-8cc2-bd17bad06f61')/appRoleAssignments/PRLbC6e4yUyM
                       wr0XutBvYZsr7FiAW3pIqP4F9944yBc]}
```

This example gets the application role assignments that have been granted to the specified service principal.

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

### -AppRoleAssignmentId
The unique identifier of appRoleAssignment

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

### -ConsistencyLevel
Indicates the requested consistency level.
Documentation URL: https://docs.microsoft.com/graph/aad-advanced-queries

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
Type: IApplicationsIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### -ServicePrincipalId
The unique identifier of servicePrincipal

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

### Microsoft.Graph.Beta.PowerShell.Models.IApplicationsIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAppRoleAssignment
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IApplicationsIdentity>`: Identity Parameter
  - `[AppId <String>]`: Alternate key of application
  - `[AppManagementPolicyId <String>]`: The unique identifier of appManagementPolicy
  - `[AppRoleAssignmentId <String>]`: The unique identifier of appRoleAssignment
  - `[ApplicationId <String>]`: The unique identifier of application
  - `[ApplicationTemplateId <String>]`: The unique identifier of applicationTemplate
  - `[ClaimsMappingPolicyId <String>]`: The unique identifier of claimsMappingPolicy
  - `[ConnectorGroupId <String>]`: The unique identifier of connectorGroup
  - `[ConnectorId <String>]`: The unique identifier of connector
  - `[DelegatedPermissionClassificationId <String>]`: The unique identifier of delegatedPermissionClassification
  - `[DirectoryDefinitionId <String>]`: The unique identifier of directoryDefinition
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EndpointId <String>]`: The unique identifier of endpoint
  - `[ExtensionPropertyId <String>]`: The unique identifier of extensionProperty
  - `[FederatedIdentityCredentialId <String>]`: The unique identifier of federatedIdentityCredential
  - `[GroupId <String>]`: The unique identifier of group
  - `[HomeRealmDiscoveryPolicyId <String>]`: The unique identifier of homeRealmDiscoveryPolicy
  - `[IPApplicationSegmentId <String>]`: The unique identifier of ipApplicationSegment
  - `[LicenseDetailsId <String>]`: The unique identifier of licenseDetails
  - `[Name <String>]`: Alternate key of federatedIdentityCredential
  - `[OAuth2PermissionGrantId <String>]`: The unique identifier of oAuth2PermissionGrant
  - `[OnPremisesAgentGroupId <String>]`: The unique identifier of onPremisesAgentGroup
  - `[OnPremisesAgentGroupId1 <String>]`: The unique identifier of onPremisesAgentGroup
  - `[OnPremisesAgentId <String>]`: The unique identifier of onPremisesAgent
  - `[OnPremisesPublishingProfileId <String>]`: The unique identifier of onPremisesPublishingProfile
  - `[PermissionGrantPreApprovalPolicyId <String>]`: The unique identifier of permissionGrantPreApprovalPolicy
  - `[PublishedResourceId <String>]`: The unique identifier of publishedResource
  - `[ServicePrincipalId <String>]`: The unique identifier of servicePrincipal
  - `[SynchronizationJobId <String>]`: The unique identifier of synchronizationJob
  - `[SynchronizationTemplateId <String>]`: The unique identifier of synchronizationTemplate
  - `[TargetDeviceGroupId <String>]`: The unique identifier of targetDeviceGroup
  - `[TokenIssuancePolicyId <String>]`: The unique identifier of tokenIssuancePolicy
  - `[TokenLifetimePolicyId <String>]`: The unique identifier of tokenLifetimePolicy
  - `[UniqueName <String>]`: Alternate key of application
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/get-mgbetaserviceprincipalapproleassignment](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/get-mgbetaserviceprincipalapproleassignment)

[https://learn.microsoft.com/graph/api/approleassignment-get?view=graph-rest-beta](https://learn.microsoft.com/graph/api/approleassignment-get?view=graph-rest-beta)

[https://learn.microsoft.com/graph/api/serviceprincipal-list-approleassignments?view=graph-rest-beta](https://learn.microsoft.com/graph/api/serviceprincipal-list-approleassignments?view=graph-rest-beta)























