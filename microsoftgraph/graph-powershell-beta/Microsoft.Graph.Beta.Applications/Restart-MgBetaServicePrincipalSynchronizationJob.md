---
external help file: Microsoft.Graph.Beta.Applications-help.xml
Module Name: Microsoft.Graph.Beta.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/restart-mgbetaserviceprincipalsynchronizationjob
schema: 2.0.0
ms.subservice: entra-applications
---

# Restart-MgBetaServicePrincipalSynchronizationJob

## SYNOPSIS
Restart a stopped synchronization job, forcing it to reprocess all the objects in the directory.
Optionally clears existing the synchronization state and previous errors.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Restart-MgServicePrincipalSynchronizationJob](/powershell/module/Microsoft.Graph.Applications/Restart-MgServicePrincipalSynchronizationJob?view=graph-powershell-1.0)

## SYNTAX

### RestartExpanded (Default)
```
Restart-MgBetaServicePrincipalSynchronizationJob -ServicePrincipalId <String> -SynchronizationJobId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Criteria <IMicrosoftGraphSynchronizationJobRestartCriteria>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Restart
```
Restart-MgBetaServicePrincipalSynchronizationJob -ServicePrincipalId <String> -SynchronizationJobId <String>
 -BodyParameter <IPaths7MrbavServiceprincipalsServiceprincipalIdSynchronizationJobsSynchronizationjobIdMicrosoftGraphRestartPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RestartViaIdentityExpanded
```
Restart-MgBetaServicePrincipalSynchronizationJob -InputObject <IApplicationsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Criteria <IMicrosoftGraphSynchronizationJobRestartCriteria>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RestartViaIdentity
```
Restart-MgBetaServicePrincipalSynchronizationJob -InputObject <IApplicationsIdentity>
 -BodyParameter <IPaths7MrbavServiceprincipalsServiceprincipalIdSynchronizationJobsSynchronizationjobIdMicrosoftGraphRestartPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Restart a stopped synchronization job, forcing it to reprocess all the objects in the directory.
Optionally clears existing the synchronization state and previous errors.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Synchronization.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Application.ReadWrite.OwnedBy, Synchronization.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	criteria = @{
		resetScope = "Watermark, Escrows, QuarantineState"
	}
}

Restart-MgBetaServicePrincipalSynchronizationJob -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId -BodyParameter $params

```
This example shows how to use the Restart-MgBetaServicePrincipalSynchronizationJob Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: RestartExpanded, RestartViaIdentityExpanded
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
Type: IPaths7MrbavServiceprincipalsServiceprincipalIdSynchronizationJobsSynchronizationjobIdMicrosoftGraphRestartPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Restart, RestartViaIdentity
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

### -Criteria
synchronizationJobRestartCriteria
To construct, see NOTES section for CRITERIA properties and create a hash table.

```yaml
Type: IMicrosoftGraphSynchronizationJobRestartCriteria
Parameter Sets: RestartExpanded, RestartViaIdentityExpanded
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
Parameter Sets: RestartViaIdentityExpanded, RestartViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
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

### -ServicePrincipalId
The unique identifier of servicePrincipal

```yaml
Type: String
Parameter Sets: RestartExpanded, Restart
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SynchronizationJobId
The unique identifier of synchronizationJob

```yaml
Type: String
Parameter Sets: RestartExpanded, Restart
Aliases:

Required: True
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

### Microsoft.Graph.Beta.PowerShell.Models.IApplicationsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IPaths7MrbavServiceprincipalsServiceprincipalIdSynchronizationJobsSynchronizationjobIdMicrosoftGraphRestartPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths7MrbavServiceprincipalsServiceprincipalIdSynchronizationJobsSynchronizationjobIdMicrosoftGraphRestartPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Criteria <IMicrosoftGraphSynchronizationJobRestartCriteria>]`: synchronizationJobRestartCriteria
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ResetScope <String>]`: synchronizationJobRestartScope

CRITERIA `<IMicrosoftGraphSynchronizationJobRestartCriteria>`: synchronizationJobRestartCriteria
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ResetScope <String>]`: synchronizationJobRestartScope

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/restart-mgbetaserviceprincipalsynchronizationjob](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/restart-mgbetaserviceprincipalsynchronizationjob)

[https://learn.microsoft.com/graph/api/synchronization-synchronizationjob-restart?view=graph-rest-beta](https://learn.microsoft.com/graph/api/synchronization-synchronizationjob-restart?view=graph-rest-beta)























