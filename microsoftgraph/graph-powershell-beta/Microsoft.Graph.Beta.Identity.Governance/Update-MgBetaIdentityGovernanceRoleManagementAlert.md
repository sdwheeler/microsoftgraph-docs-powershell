---
external help file: Microsoft.Graph.Beta.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Beta.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/update-mgbetaidentitygovernancerolemanagementalert
schema: 2.0.0
---

# Update-MgBetaIdentityGovernanceRoleManagementAlert

## SYNOPSIS
Invoke action refresh

## SYNTAX

### RefreshExpanded (Default)
```
Update-MgBetaIdentityGovernanceRoleManagementAlert [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ScopeId <String>] [-ScopeType <String>] [-Headers <IDictionary>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateExpanded
```
Update-MgBetaIdentityGovernanceRoleManagementAlert -UnifiedRoleManagementAlertId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-ScopeId <String>]
 [-ScopeType <String>] [-AlertConfiguration <IMicrosoftGraphUnifiedRoleManagementAlertConfiguration>]
 [-AlertDefinition <IMicrosoftGraphUnifiedRoleManagementAlertDefinition>] [-AlertDefinitionId <String>]
 [-AlertIncidents <IMicrosoftGraphUnifiedRoleManagementAlertIncident[]>] [-Id <String>]
 [-IncidentCount <Int32>] [-IsActive] [-LastModifiedDateTime <DateTime>] [-LastScannedDateTime <DateTime>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaIdentityGovernanceRoleManagementAlert -UnifiedRoleManagementAlertId <String>
 [-ResponseHeadersVariable <String>] -BodyParameter <IMicrosoftGraphUnifiedRoleManagementAlert>
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Refresh
```
Update-MgBetaIdentityGovernanceRoleManagementAlert -UnifiedRoleManagementAlertId <String>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaIdentityGovernanceRoleManagementAlert -InputObject <IIdentityGovernanceIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-ScopeId <String>]
 [-ScopeType <String>] [-AlertConfiguration <IMicrosoftGraphUnifiedRoleManagementAlertConfiguration>]
 [-AlertDefinition <IMicrosoftGraphUnifiedRoleManagementAlertDefinition>] [-AlertDefinitionId <String>]
 [-AlertIncidents <IMicrosoftGraphUnifiedRoleManagementAlertIncident[]>] [-Id <String>]
 [-IncidentCount <Int32>] [-IsActive] [-LastModifiedDateTime <DateTime>] [-LastScannedDateTime <DateTime>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaIdentityGovernanceRoleManagementAlert -InputObject <IIdentityGovernanceIdentity>
 [-ResponseHeadersVariable <String>] -BodyParameter <IMicrosoftGraphUnifiedRoleManagementAlert>
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RefreshViaIdentity
```
Update-MgBetaIdentityGovernanceRoleManagementAlert -InputObject <IIdentityGovernanceIdentity>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Refresh1
```
Update-MgBetaIdentityGovernanceRoleManagementAlert [-ResponseHeadersVariable <String>]
 -Body <IPaths1O7WbujIdentitygovernanceRolemanagementalertsAlertsMicrosoftGraphRefreshPostRequestbodyContentApplicationJsonSchema>
 [-Headers <IDictionary>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Invoke action refresh

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: RefreshExpanded, UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AlertConfiguration
unifiedRoleManagementAlertConfiguration
To construct, see NOTES section for ALERTCONFIGURATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleManagementAlertConfiguration
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AlertDefinition
unifiedRoleManagementAlertDefinition
To construct, see NOTES section for ALERTDEFINITION properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleManagementAlertDefinition
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AlertDefinitionId
The identifier of an alert definition.
Supports $filter (eq, ne).

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

### -AlertIncidents
Represents the incidents of this type of alert that have been triggered in Privileged Identity Management (PIM) for Microsoft Entra roles in the tenant.
Supports $expand.
To construct, see NOTES section for ALERTINCIDENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleManagementAlertIncident[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Body

To construct, see NOTES section for BODY properties and create a hash table.

```yaml
Type: IPaths1O7WbujIdentitygovernanceRolemanagementalertsAlertsMicrosoftGraphRefreshPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Refresh1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BodyParameter
unifiedRoleManagementAlert
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleManagementAlert
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

### -IncidentCount
The number of incidents triggered in the tenant and relating to the alert.
Can only be a positive integer.

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IIdentityGovernanceIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity, RefreshViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsActive
false by default.
true if the alert is active.

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

### -LastModifiedDateTime
The date time when the alert configuration was updated or new incidents generated.

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

### -LastScannedDateTime
The date time when the tenant was last scanned for incidents that trigger this alert.

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

### -PassThru
Returns true when the command succeeds

```yaml
Type: SwitchParameter
Parameter Sets: RefreshExpanded, Refresh, RefreshViaIdentity, Refresh1
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

### -ScopeId


```yaml
Type: String
Parameter Sets: RefreshExpanded, UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScopeType


```yaml
Type: String
Parameter Sets: RefreshExpanded, UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UnifiedRoleManagementAlertId
The unique identifier of unifiedRoleManagementAlert

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update, Refresh
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

### Microsoft.Graph.Beta.PowerShell.Models.IIdentityGovernanceIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUnifiedRoleManagementAlert
### Microsoft.Graph.Beta.PowerShell.Models.IPaths1O7WbujIdentitygovernanceRolemanagementalertsAlertsMicrosoftGraphRefreshPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUnifiedRoleManagementAlert
### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ALERTCONFIGURATION `<IMicrosoftGraphUnifiedRoleManagementAlertConfiguration>`: unifiedRoleManagementAlertConfiguration
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AlertDefinition <IMicrosoftGraphUnifiedRoleManagementAlertDefinition>]`: unifiedRoleManagementAlertDefinition
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Description <String>]`: The description of the alert.
    - `[DisplayName <String>]`: The friendly display name that renders in Privileged Identity Management (PIM) alerts in the Microsoft Entra admin center.
    - `[HowToPrevent <String>]`: Long-form text that indicates the ways to prevent the alert from being triggered in your tenant.
    - `[IsConfigurable <Boolean?>]`: true if the alert configuration can be customized in the tenant, and false otherwise.
For example, the number and percentage thresholds of the 'There are too many global administrators' alert can be configured by users, while the 'This organization doesn't have Microsoft Entra ID P2' can't be configured, because the criteria are restricted.
    - `[IsRemediatable <Boolean?>]`: true if the alert can be remediated, and false otherwise.
    - `[MitigationSteps <String>]`: The methods to mitigate the alert when it's triggered in the tenant.
For example, to mitigate the 'There are too many global administrators', you could remove redundant privileged role assignments.
    - `[ScopeId <String>]`: The identifier of the scope where the alert is related.
/ is the only supported one for the tenant.
Supports $filter (eq, ne).
    - `[ScopeType <String>]`: The type of scope where the alert is created.
DirectoryRole is the only currently supported scope type for Microsoft Entra roles.
    - `[SecurityImpact <String>]`: Security impact of the alert.
For example, it could be information leaks or unauthorized access.
    - `[SeverityLevel <String>]`: alertSeverity
  - `[AlertDefinitionId <String>]`: The identifier of an alert definition.
Supports $filter (eq, ne).
  - `[IsEnabled <Boolean?>]`: true if the alert is enabled.
Setting it to false disables PIM scanning the tenant to identify instances that trigger the alert.
  - `[ScopeId <String>]`: The identifier of the scope to which the alert is related.
Only / is supported to represent the tenant scope.
Supports $filter (eq, ne).
  - `[ScopeType <String>]`: The type of scope where the alert is created.
DirectoryRole is the only currently supported scope type for Microsoft Entra roles.

ALERTDEFINITION `<IMicrosoftGraphUnifiedRoleManagementAlertDefinition>`: unifiedRoleManagementAlertDefinition
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Description <String>]`: The description of the alert.
  - `[DisplayName <String>]`: The friendly display name that renders in Privileged Identity Management (PIM) alerts in the Microsoft Entra admin center.
  - `[HowToPrevent <String>]`: Long-form text that indicates the ways to prevent the alert from being triggered in your tenant.
  - `[IsConfigurable <Boolean?>]`: true if the alert configuration can be customized in the tenant, and false otherwise.
For example, the number and percentage thresholds of the 'There are too many global administrators' alert can be configured by users, while the 'This organization doesn't have Microsoft Entra ID P2' can't be configured, because the criteria are restricted.
  - `[IsRemediatable <Boolean?>]`: true if the alert can be remediated, and false otherwise.
  - `[MitigationSteps <String>]`: The methods to mitigate the alert when it's triggered in the tenant.
For example, to mitigate the 'There are too many global administrators', you could remove redundant privileged role assignments.
  - `[ScopeId <String>]`: The identifier of the scope where the alert is related.
/ is the only supported one for the tenant.
Supports $filter (eq, ne).
  - `[ScopeType <String>]`: The type of scope where the alert is created.
DirectoryRole is the only currently supported scope type for Microsoft Entra roles.
  - `[SecurityImpact <String>]`: Security impact of the alert.
For example, it could be information leaks or unauthorized access.
  - `[SeverityLevel <String>]`: alertSeverity

ALERTINCIDENTS `<IMicrosoftGraphUnifiedRoleManagementAlertIncident- `[]`>`: Represents the incidents of this type of alert that have been triggered in Privileged Identity Management (PIM) for Microsoft Entra roles in the tenant.
Supports $expand.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

BODY `<IPaths1O7WbujIdentitygovernanceRolemanagementalertsAlertsMicrosoftGraphRefreshPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ScopeId <String>]`: 
  - `[ScopeType <String>]`: 

BODYPARAMETER `<IMicrosoftGraphUnifiedRoleManagementAlert>`: unifiedRoleManagementAlert
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AlertConfiguration <IMicrosoftGraphUnifiedRoleManagementAlertConfiguration>]`: unifiedRoleManagementAlertConfiguration
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AlertDefinition <IMicrosoftGraphUnifiedRoleManagementAlertDefinition>]`: unifiedRoleManagementAlertDefinition
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Description <String>]`: The description of the alert.
      - `[DisplayName <String>]`: The friendly display name that renders in Privileged Identity Management (PIM) alerts in the Microsoft Entra admin center.
      - `[HowToPrevent <String>]`: Long-form text that indicates the ways to prevent the alert from being triggered in your tenant.
      - `[IsConfigurable <Boolean?>]`: true if the alert configuration can be customized in the tenant, and false otherwise.
For example, the number and percentage thresholds of the 'There are too many global administrators' alert can be configured by users, while the 'This organization doesn't have Microsoft Entra ID P2' can't be configured, because the criteria are restricted.
      - `[IsRemediatable <Boolean?>]`: true if the alert can be remediated, and false otherwise.
      - `[MitigationSteps <String>]`: The methods to mitigate the alert when it's triggered in the tenant.
For example, to mitigate the 'There are too many global administrators', you could remove redundant privileged role assignments.
      - `[ScopeId <String>]`: The identifier of the scope where the alert is related.
/ is the only supported one for the tenant.
Supports $filter (eq, ne).
      - `[ScopeType <String>]`: The type of scope where the alert is created.
DirectoryRole is the only currently supported scope type for Microsoft Entra roles.
      - `[SecurityImpact <String>]`: Security impact of the alert.
For example, it could be information leaks or unauthorized access.
      - `[SeverityLevel <String>]`: alertSeverity
    - `[AlertDefinitionId <String>]`: The identifier of an alert definition.
Supports $filter (eq, ne).
    - `[IsEnabled <Boolean?>]`: true if the alert is enabled.
Setting it to false disables PIM scanning the tenant to identify instances that trigger the alert.
    - `[ScopeId <String>]`: The identifier of the scope to which the alert is related.
Only / is supported to represent the tenant scope.
Supports $filter (eq, ne).
    - `[ScopeType <String>]`: The type of scope where the alert is created.
DirectoryRole is the only currently supported scope type for Microsoft Entra roles.
  - `[AlertDefinition <IMicrosoftGraphUnifiedRoleManagementAlertDefinition>]`: unifiedRoleManagementAlertDefinition
  - `[AlertDefinitionId <String>]`: The identifier of an alert definition.
Supports $filter (eq, ne).
  - `[AlertIncidents <IMicrosoftGraphUnifiedRoleManagementAlertIncident- `[]`>]`: Represents the incidents of this type of alert that have been triggered in Privileged Identity Management (PIM) for Microsoft Entra roles in the tenant.
Supports $expand.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[IncidentCount <Int32?>]`: The number of incidents triggered in the tenant and relating to the alert.
Can only be a positive integer.
  - `[IsActive <Boolean?>]`: false by default.
true if the alert is active.
  - `[LastModifiedDateTime <DateTime?>]`: The date time when the alert configuration was updated or new incidents generated.
  - `[LastScannedDateTime <DateTime?>]`: The date time when the tenant was last scanned for incidents that trigger this alert.
  - `[ScopeId <String>]`: The identifier of the scope where the alert is related.
/ is the only supported one for the tenant.
Supports $filter (eq, ne).
  - `[ScopeType <String>]`: The type of scope where the alert is created.
DirectoryRole is the only currently supported scope type for Microsoft Entra roles.

INPUTOBJECT `<IIdentityGovernanceIdentity>`: Identity Parameter
  - `[AccessPackageAssignmentId <String>]`: The unique identifier of accessPackageAssignment
  - `[AccessPackageAssignmentPolicyId <String>]`: The unique identifier of accessPackageAssignmentPolicy
  - `[AccessPackageAssignmentRequestId <String>]`: The unique identifier of accessPackageAssignmentRequest
  - `[AccessPackageAssignmentResourceRoleId <String>]`: The unique identifier of accessPackageAssignmentResourceRole
  - `[AccessPackageCatalogId <String>]`: The unique identifier of accessPackageCatalog
  - `[AccessPackageId <String>]`: The unique identifier of accessPackage
  - `[AccessPackageId1 <String>]`: The unique identifier of accessPackage
  - `[AccessPackageResourceEnvironmentId <String>]`: The unique identifier of accessPackageResourceEnvironment
  - `[AccessPackageResourceId <String>]`: The unique identifier of accessPackageResource
  - `[AccessPackageResourceRequestId <String>]`: The unique identifier of accessPackageResourceRequest
  - `[AccessPackageResourceRoleId <String>]`: The unique identifier of accessPackageResourceRole
  - `[AccessPackageResourceRoleScopeId <String>]`: The unique identifier of accessPackageResourceRoleScope
  - `[AccessPackageResourceScopeId <String>]`: The unique identifier of accessPackageResourceScope
  - `[AccessPackageSubjectId <String>]`: The unique identifier of accessPackageSubject
  - `[AccessReviewDecisionId <String>]`: The unique identifier of accessReviewDecision
  - `[AccessReviewHistoryDefinitionId <String>]`: The unique identifier of accessReviewHistoryDefinition
  - `[AccessReviewHistoryInstanceId <String>]`: The unique identifier of accessReviewHistoryInstance
  - `[AccessReviewId <String>]`: The unique identifier of accessReview
  - `[AccessReviewId1 <String>]`: The unique identifier of accessReview
  - `[AccessReviewInstanceDecisionItemId <String>]`: The unique identifier of accessReviewInstanceDecisionItem
  - `[AccessReviewInstanceDecisionItemId1 <String>]`: The unique identifier of accessReviewInstanceDecisionItem
  - `[AccessReviewInstanceId <String>]`: The unique identifier of accessReviewInstance
  - `[AccessReviewReviewerId <String>]`: The unique identifier of accessReviewReviewer
  - `[AccessReviewScheduleDefinitionId <String>]`: The unique identifier of accessReviewScheduleDefinition
  - `[AccessReviewStageId <String>]`: The unique identifier of accessReviewStage
  - `[AgreementAcceptanceId <String>]`: The unique identifier of agreementAcceptance
  - `[AgreementFileLocalizationId <String>]`: The unique identifier of agreementFileLocalization
  - `[AgreementFileVersionId <String>]`: The unique identifier of agreementFileVersion
  - `[AgreementId <String>]`: The unique identifier of agreement
  - `[AppConsentRequestId <String>]`: The unique identifier of appConsentRequest
  - `[ApprovalId <String>]`: The unique identifier of approval
  - `[ApprovalStepId <String>]`: The unique identifier of approvalStep
  - `[BusinessFlowTemplateId <String>]`: The unique identifier of businessFlowTemplate
  - `[ConnectedOrganizationId <String>]`: The unique identifier of connectedOrganization
  - `[CustomAccessPackageWorkflowExtensionId <String>]`: The unique identifier of customAccessPackageWorkflowExtension
  - `[CustomCalloutExtensionId <String>]`: The unique identifier of customCalloutExtension
  - `[CustomExtensionHandlerId <String>]`: The unique identifier of customExtensionHandler
  - `[CustomExtensionStageSettingId <String>]`: The unique identifier of customExtensionStageSetting
  - `[CustomTaskExtensionId <String>]`: The unique identifier of customTaskExtension
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EndDateTime <DateTime?>]`: Usage: endDateTime={endDateTime}
  - `[FindingId <String>]`: The unique identifier of finding
  - `[GovernanceInsightId <String>]`: The unique identifier of governanceInsight
  - `[GovernanceResourceId <String>]`: The unique identifier of governanceResource
  - `[GovernanceRoleAssignmentId <String>]`: The unique identifier of governanceRoleAssignment
  - `[GovernanceRoleAssignmentRequestId <String>]`: The unique identifier of governanceRoleAssignmentRequest
  - `[GovernanceRoleDefinitionId <String>]`: The unique identifier of governanceRoleDefinition
  - `[GovernanceRoleSettingId <String>]`: The unique identifier of governanceRoleSetting
  - `[IncompatibleAccessPackageId <String>]`: Usage: incompatibleAccessPackageId='{incompatibleAccessPackageId}'
  - `[LongRunningOperationId <String>]`: The unique identifier of longRunningOperation
  - `[ObjectId <String>]`: Alternate key of accessPackageSubject
  - `[On <String>]`: Usage: on='{on}'
  - `[PermissionsCreepIndexDistributionId <String>]`: The unique identifier of permissionsCreepIndexDistribution
  - `[PermissionsRequestChangeId <String>]`: The unique identifier of permissionsRequestChange
  - `[PrivilegedAccessGroupAssignmentScheduleId <String>]`: The unique identifier of privilegedAccessGroupAssignmentSchedule
  - `[PrivilegedAccessGroupAssignmentScheduleInstanceId <String>]`: The unique identifier of privilegedAccessGroupAssignmentScheduleInstance
  - `[PrivilegedAccessGroupAssignmentScheduleRequestId <String>]`: The unique identifier of privilegedAccessGroupAssignmentScheduleRequest
  - `[PrivilegedAccessGroupEligibilityScheduleId <String>]`: The unique identifier of privilegedAccessGroupEligibilitySchedule
  - `[PrivilegedAccessGroupEligibilityScheduleInstanceId <String>]`: The unique identifier of privilegedAccessGroupEligibilityScheduleInstance
  - `[PrivilegedAccessGroupEligibilityScheduleRequestId <String>]`: The unique identifier of privilegedAccessGroupEligibilityScheduleRequest
  - `[PrivilegedAccessId <String>]`: The unique identifier of privilegedAccess
  - `[PrivilegedApprovalId <String>]`: The unique identifier of privilegedApproval
  - `[PrivilegedOperationEventId <String>]`: The unique identifier of privilegedOperationEvent
  - `[PrivilegedRoleAssignmentId <String>]`: The unique identifier of privilegedRoleAssignment
  - `[PrivilegedRoleAssignmentId1 <String>]`: The unique identifier of privilegedRoleAssignment
  - `[PrivilegedRoleAssignmentRequestId <String>]`: The unique identifier of privilegedRoleAssignmentRequest
  - `[PrivilegedRoleId <String>]`: The unique identifier of privilegedRole
  - `[ProgramControlId <String>]`: The unique identifier of programControl
  - `[ProgramControlId1 <String>]`: The unique identifier of programControl
  - `[ProgramControlTypeId <String>]`: The unique identifier of programControlType
  - `[ProgramId <String>]`: The unique identifier of program
  - `[RbacApplicationId <String>]`: The unique identifier of rbacApplication
  - `[RunId <String>]`: The unique identifier of run
  - `[StartDateTime <DateTime?>]`: Usage: startDateTime={startDateTime}
  - `[TaskDefinitionId <String>]`: The unique identifier of taskDefinition
  - `[TaskId <String>]`: The unique identifier of task
  - `[TaskProcessingResultId <String>]`: The unique identifier of taskProcessingResult
  - `[TaskReportId <String>]`: The unique identifier of taskReport
  - `[UnifiedRbacResourceActionId <String>]`: The unique identifier of unifiedRbacResourceAction
  - `[UnifiedRbacResourceNamespaceId <String>]`: The unique identifier of unifiedRbacResourceNamespace
  - `[UnifiedRoleAssignmentId <String>]`: The unique identifier of unifiedRoleAssignment
  - `[UnifiedRoleAssignmentScheduleId <String>]`: The unique identifier of unifiedRoleAssignmentSchedule
  - `[UnifiedRoleAssignmentScheduleInstanceId <String>]`: The unique identifier of unifiedRoleAssignmentScheduleInstance
  - `[UnifiedRoleAssignmentScheduleRequestId <String>]`: The unique identifier of unifiedRoleAssignmentScheduleRequest
  - `[UnifiedRoleDefinitionId <String>]`: The unique identifier of unifiedRoleDefinition
  - `[UnifiedRoleDefinitionId1 <String>]`: The unique identifier of unifiedRoleDefinition
  - `[UnifiedRoleEligibilityScheduleId <String>]`: The unique identifier of unifiedRoleEligibilitySchedule
  - `[UnifiedRoleEligibilityScheduleInstanceId <String>]`: The unique identifier of unifiedRoleEligibilityScheduleInstance
  - `[UnifiedRoleEligibilityScheduleRequestId <String>]`: The unique identifier of unifiedRoleEligibilityScheduleRequest
  - `[UnifiedRoleManagementAlertConfigurationId <String>]`: The unique identifier of unifiedRoleManagementAlertConfiguration
  - `[UnifiedRoleManagementAlertDefinitionId <String>]`: The unique identifier of unifiedRoleManagementAlertDefinition
  - `[UnifiedRoleManagementAlertId <String>]`: The unique identifier of unifiedRoleManagementAlert
  - `[UnifiedRoleManagementAlertIncidentId <String>]`: The unique identifier of unifiedRoleManagementAlertIncident
  - `[UniqueName <String>]`: Alternate key of accessPackageCatalog
  - `[UserConsentRequestId <String>]`: The unique identifier of userConsentRequest
  - `[UserId <String>]`: The unique identifier of user
  - `[UserProcessingResultId <String>]`: The unique identifier of userProcessingResult
  - `[WorkflowId <String>]`: The unique identifier of workflow
  - `[WorkflowTemplateId <String>]`: The unique identifier of workflowTemplate
  - `[WorkflowVersionNumber <Int32?>]`: The unique identifier of workflowVersion

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/update-mgbetaidentitygovernancerolemanagementalert](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/update-mgbetaidentitygovernancerolemanagementalert)

[https://learn.microsoft.com/graph/api/unifiedrolemanagementalert-refresh?view=graph-rest-beta](https://learn.microsoft.com/graph/api/unifiedrolemanagementalert-refresh?view=graph-rest-beta)
























