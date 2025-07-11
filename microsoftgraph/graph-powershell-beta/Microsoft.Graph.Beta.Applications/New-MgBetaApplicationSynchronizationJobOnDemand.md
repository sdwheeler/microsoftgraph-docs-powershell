---
external help file: Microsoft.Graph.Beta.Applications-help.xml
Module Name: Microsoft.Graph.Beta.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/new-mgbetaapplicationsynchronizationjobondemand
schema: 2.0.0
ms.subservice: entra-applications
---

# New-MgBetaApplicationSynchronizationJobOnDemand

## SYNOPSIS
Select a user and provision the account on-demand.
The rate limit for this API is 5 requests per 10 seconds.
No user or group will be provisioned on-demand that would not have been provisioned through the regular provisioning cycles.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgApplicationSynchronizationJobOnDemand](/powershell/module/Microsoft.Graph.Applications/New-MgApplicationSynchronizationJobOnDemand?view=graph-powershell-1.0)

## SYNTAX

### ProvisionExpanded (Default)
```
New-MgBetaApplicationSynchronizationJobOnDemand -ApplicationId <String> -SynchronizationJobId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Parameters <IMicrosoftGraphSynchronizationJobApplicationParameters[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Provision
```
New-MgBetaApplicationSynchronizationJobOnDemand -ApplicationId <String> -SynchronizationJobId <String>
 -BodyParameter <IPaths1A5O87GApplicationsApplicationIdSynchronizationJobsSynchronizationjobIdMicrosoftGraphProvisionondemandPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### ProvisionViaIdentityExpanded
```
New-MgBetaApplicationSynchronizationJobOnDemand -InputObject <IApplicationsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Parameters <IMicrosoftGraphSynchronizationJobApplicationParameters[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ProvisionViaIdentity
```
New-MgBetaApplicationSynchronizationJobOnDemand -InputObject <IApplicationsIdentity>
 -BodyParameter <IPaths1A5O87GApplicationsApplicationIdSynchronizationJobsSynchronizationjobIdMicrosoftGraphProvisionondemandPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Select a user and provision the account on-demand.
The rate limit for this API is 5 requests per 10 seconds.
No user or group will be provisioned on-demand that would not have been provisioned through the regular provisioning cycles.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: ProvisionExpanded, ProvisionViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationId
The unique identifier of application

```yaml
Type: String
Parameter Sets: ProvisionExpanded, Provision
Aliases: ObjectId

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter

To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths1A5O87GApplicationsApplicationIdSynchronizationJobsSynchronizationjobIdMicrosoftGraphProvisionondemandPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Provision, ProvisionViaIdentity
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
Parameter Sets: ProvisionViaIdentityExpanded, ProvisionViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Parameters

To construct, see NOTES section for PARAMETERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSynchronizationJobApplicationParameters[]
Parameter Sets: ProvisionExpanded, ProvisionViaIdentityExpanded
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

### -SynchronizationJobId
The unique identifier of synchronizationJob

```yaml
Type: String
Parameter Sets: ProvisionExpanded, Provision
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
### Microsoft.Graph.Beta.PowerShell.Models.IPaths1A5O87GApplicationsApplicationIdSynchronizationJobsSynchronizationjobIdMicrosoftGraphProvisionondemandPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphStringKeyStringValuePair
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths1A5O87GApplicationsApplicationIdSynchronizationJobsSynchronizationjobIdMicrosoftGraphProvisionondemandPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Parameters <IMicrosoftGraphSynchronizationJobApplicationParameters- `[]`>]`: 
    - `[RuleId <String>]`: The identifier of the synchronizationRule to be applied.
This rule ID is defined in the schema for a given synchronization job or template.
    - `[Subjects <IMicrosoftGraphSynchronizationJobSubject- `[]`>]`: The identifiers of one or more objects to which a synchronizationJob is to be applied.
      - `[Links <IMicrosoftGraphSynchronizationLinkedObjects>]`: synchronizationLinkedObjects
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Manager <IMicrosoftGraphSynchronizationJobSubject>]`: synchronizationJobSubject
        - `[Members <IMicrosoftGraphSynchronizationJobSubject- `[]`>]`: All group members that you would like to provision.
        - `[Owners <IMicrosoftGraphSynchronizationJobSubject- `[]`>]`: 
      - `[ObjectId <String>]`: The identifier of an object to which a synchronizationJob is to be applied.
Can be one of the following: An onPremisesDistinguishedName for synchronization from Active Directory to Azure AD.The user ID for synchronization from Microsoft Entra ID to a third-party.The Worker ID of the Workday worker for synchronization from Workday to either Active Directory or Azure AD.
      - `[ObjectTypeName <String>]`: The type of the object to which a synchronizationJob is to be applied.
Can be one of the following: user for synchronizing between Active Directory and Azure AD.User for synchronizing a user between Microsoft Entra ID and a third-party application.
Worker for synchronization a user between Workday and either Active Directory or Azure AD.Group for synchronizing a group between Microsoft Entra ID and a third-party application.

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

PARAMETERS `<IMicrosoftGraphSynchronizationJobApplicationParameters- `[]`>`: .
  - `[RuleId <String>]`: The identifier of the synchronizationRule to be applied.
This rule ID is defined in the schema for a given synchronization job or template.
  - `[Subjects <IMicrosoftGraphSynchronizationJobSubject- `[]`>]`: The identifiers of one or more objects to which a synchronizationJob is to be applied.
    - `[Links <IMicrosoftGraphSynchronizationLinkedObjects>]`: synchronizationLinkedObjects
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Manager <IMicrosoftGraphSynchronizationJobSubject>]`: synchronizationJobSubject
      - `[Members <IMicrosoftGraphSynchronizationJobSubject- `[]`>]`: All group members that you would like to provision.
      - `[Owners <IMicrosoftGraphSynchronizationJobSubject- `[]`>]`: 
    - `[ObjectId <String>]`: The identifier of an object to which a synchronizationJob is to be applied.
Can be one of the following: An onPremisesDistinguishedName for synchronization from Active Directory to Azure AD.The user ID for synchronization from Microsoft Entra ID to a third-party.The Worker ID of the Workday worker for synchronization from Workday to either Active Directory or Azure AD.
    - `[ObjectTypeName <String>]`: The type of the object to which a synchronizationJob is to be applied.
Can be one of the following: user for synchronizing between Active Directory and Azure AD.User for synchronizing a user between Microsoft Entra ID and a third-party application.
Worker for synchronization a user between Workday and either Active Directory or Azure AD.Group for synchronizing a group between Microsoft Entra ID and a third-party application.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/new-mgbetaapplicationsynchronizationjobondemand](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/new-mgbetaapplicationsynchronizationjobondemand)

[https://learn.microsoft.com/graph/api/synchronization-synchronizationjob-provisionondemand?view=graph-rest-beta](https://learn.microsoft.com/graph/api/synchronization-synchronizationjob-provisionondemand?view=graph-rest-beta)
























