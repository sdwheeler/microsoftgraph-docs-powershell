---
external help file: Microsoft.Graph.Beta.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Beta.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/update-mgbetaidentitygovernancelifecycleworkflowtemplatetaskprocessingresultsubjectmailboxsetting
schema: 2.0.0
---

# Update-MgBetaIdentityGovernanceLifecycleWorkflowTemplateTaskProcessingResultSubjectMailboxSetting

## SYNOPSIS
Update property mailboxSettings value.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgIdentityGovernanceLifecycleWorkflowTemplateTaskProcessingResultSubjectMailboxSetting](/powershell/module/Microsoft.Graph.Identity.Governance/Update-MgIdentityGovernanceLifecycleWorkflowTemplateTaskProcessingResultSubjectMailboxSetting?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaIdentityGovernanceLifecycleWorkflowTemplateTaskProcessingResultSubjectMailboxSetting
 -TaskId <String> -TaskProcessingResultId <String> -WorkflowTemplateId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-ArchiveFolder <String>]
 [-AutomaticRepliesSetting <IMicrosoftGraphAutomaticRepliesSetting>] [-DateFormat <String>]
 [-DelegateMeetingMessageDeliveryOptions <String>] [-Language <IMicrosoftGraphLocaleInfo>]
 [-TimeFormat <String>] [-TimeZone <String>] [-UserPurpose <String>] [-UserPurposeV2 <String>]
 [-WorkingHours <IMicrosoftGraphWorkingHours>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaIdentityGovernanceLifecycleWorkflowTemplateTaskProcessingResultSubjectMailboxSetting
 -TaskId <String> -TaskProcessingResultId <String> -WorkflowTemplateId <String>
 -BodyParameter <IMicrosoftGraphMailboxSettings> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaIdentityGovernanceLifecycleWorkflowTemplateTaskProcessingResultSubjectMailboxSetting
 -InputObject <IIdentityGovernanceIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ArchiveFolder <String>]
 [-AutomaticRepliesSetting <IMicrosoftGraphAutomaticRepliesSetting>] [-DateFormat <String>]
 [-DelegateMeetingMessageDeliveryOptions <String>] [-Language <IMicrosoftGraphLocaleInfo>]
 [-TimeFormat <String>] [-TimeZone <String>] [-UserPurpose <String>] [-UserPurposeV2 <String>]
 [-WorkingHours <IMicrosoftGraphWorkingHours>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaIdentityGovernanceLifecycleWorkflowTemplateTaskProcessingResultSubjectMailboxSetting
 -InputObject <IIdentityGovernanceIdentity> -BodyParameter <IMicrosoftGraphMailboxSettings>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update property mailboxSettings value.

## EXAMPLES

## PARAMETERS

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

### -ArchiveFolder
Folder ID of an archive folder for the user.
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

### -AutomaticRepliesSetting
automaticRepliesSetting
To construct, see NOTES section for AUTOMATICREPLIESSETTING properties and create a hash table.

```yaml
Type: IMicrosoftGraphAutomaticRepliesSetting
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
mailboxSettings
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphMailboxSettings
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

### -DateFormat
The date format for the user's mailbox.

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

### -DelegateMeetingMessageDeliveryOptions
delegateMeetingMessageDeliveryOptions

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IIdentityGovernanceIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Language
localeInfo
To construct, see NOTES section for LANGUAGE properties and create a hash table.

```yaml
Type: IMicrosoftGraphLocaleInfo
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

### -TaskId
The unique identifier of task

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

### -TaskProcessingResultId
The unique identifier of taskProcessingResult

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

### -TimeFormat
The time format for the user's mailbox.

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

### -TimeZone
The default time zone for the user's mailbox.

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

### -UserPurpose
userPurpose

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

### -UserPurposeV2
mailboxRecipientType

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

### -WorkflowTemplateId
The unique identifier of workflowTemplate

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

### -WorkingHours
workingHours
To construct, see NOTES section for WORKINGHOURS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWorkingHours
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

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
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMailboxSettings
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMailboxSettings
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

AUTOMATICREPLIESSETTING `<IMicrosoftGraphAutomaticRepliesSetting>`: automaticRepliesSetting
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ExternalAudience <String>]`: externalAudienceScope
  - `[ExternalReplyMessage <String>]`: The automatic reply to send to the specified external audience, if Status is AlwaysEnabled or Scheduled.
  - `[InternalReplyMessage <String>]`: The automatic reply to send to the audience internal to the signed-in user's organization, if Status is AlwaysEnabled or Scheduled.
  - `[ScheduledEndDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
    - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
  - `[ScheduledStartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
  - `[Status <String>]`: automaticRepliesStatus

BODYPARAMETER `<IMicrosoftGraphMailboxSettings>`: mailboxSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ArchiveFolder <String>]`: Folder ID of an archive folder for the user.
Read-only.
  - `[AutomaticRepliesSetting <IMicrosoftGraphAutomaticRepliesSetting>]`: automaticRepliesSetting
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ExternalAudience <String>]`: externalAudienceScope
    - `[ExternalReplyMessage <String>]`: The automatic reply to send to the specified external audience, if Status is AlwaysEnabled or Scheduled.
    - `[InternalReplyMessage <String>]`: The automatic reply to send to the audience internal to the signed-in user's organization, if Status is AlwaysEnabled or Scheduled.
    - `[ScheduledEndDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
      - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
    - `[ScheduledStartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[Status <String>]`: automaticRepliesStatus
  - `[DateFormat <String>]`: The date format for the user's mailbox.
  - `[DelegateMeetingMessageDeliveryOptions <String>]`: delegateMeetingMessageDeliveryOptions
  - `[Language <IMicrosoftGraphLocaleInfo>]`: localeInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: A name representing the user's locale in natural language, for example, 'English (United States)'.
    - `[Locale <String>]`: A locale representation for the user, which includes the user's preferred language and country/region.
For example, 'en-us'.
The language component follows 2-letter codes as defined in ISO 639-1, and the country component follows 2-letter codes as defined in ISO 3166-1 alpha-2.
  - `[TimeFormat <String>]`: The time format for the user's mailbox.
  - `[TimeZone <String>]`: The default time zone for the user's mailbox.
  - `[UserPurpose <String>]`: userPurpose
  - `[UserPurposeV2 <String>]`: mailboxRecipientType
  - `[WorkingHours <IMicrosoftGraphWorkingHours>]`: workingHours
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DaysOfWeek <String- `[]`>]`: The days of the week on which the user works.
    - `[EndTime <String>]`: The time of the day that the user stops working.
    - `[StartTime <String>]`: The time of the day that the user starts working.
    - `[TimeZone <IMicrosoftGraphTimeZoneBase>]`: timeZoneBase
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Name <String>]`: The name of a time zone.
It can be a standard time zone name such as 'Hawaii-Aleutian Standard Time', or 'Customized Time Zone' for a custom time zone.

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

LANGUAGE `<IMicrosoftGraphLocaleInfo>`: localeInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DisplayName <String>]`: A name representing the user's locale in natural language, for example, 'English (United States)'.
  - `[Locale <String>]`: A locale representation for the user, which includes the user's preferred language and country/region.
For example, 'en-us'.
The language component follows 2-letter codes as defined in ISO 639-1, and the country component follows 2-letter codes as defined in ISO 3166-1 alpha-2.

WORKINGHOURS `<IMicrosoftGraphWorkingHours>`: workingHours
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DaysOfWeek <String- `[]`>]`: The days of the week on which the user works.
  - `[EndTime <String>]`: The time of the day that the user stops working.
  - `[StartTime <String>]`: The time of the day that the user starts working.
  - `[TimeZone <IMicrosoftGraphTimeZoneBase>]`: timeZoneBase
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Name <String>]`: The name of a time zone.
It can be a standard time zone name such as 'Hawaii-Aleutian Standard Time', or 'Customized Time Zone' for a custom time zone.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/update-mgbetaidentitygovernancelifecycleworkflowtemplatetaskprocessingresultsubjectmailboxsetting](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/update-mgbetaidentitygovernancelifecycleworkflowtemplatetaskprocessingresultsubjectmailboxsetting)
























