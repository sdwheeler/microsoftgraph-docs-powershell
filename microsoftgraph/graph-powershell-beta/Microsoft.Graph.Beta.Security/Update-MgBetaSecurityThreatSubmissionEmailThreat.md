---
external help file: Microsoft.Graph.Beta.Security-help.xml
Module Name: Microsoft.Graph.Beta.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/update-mgbetasecuritythreatsubmissionemailthreat
schema: 2.0.0
---

# Update-MgBetaSecurityThreatSubmissionEmailThreat

## SYNOPSIS
Update the navigation property emailThreats in security

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaSecurityThreatSubmissionEmailThreat -EmailThreatSubmissionId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AdminReview <IMicrosoftGraphSecuritySubmissionAdminReview>]
 [-AttackSimulationInfo <IMicrosoftGraphSecurityAttackSimulationInfo>] [-Category <String>]
 [-ClientSource <String>] [-ContentType <String>] [-CreatedBy <IMicrosoftGraphSecuritySubmissionUserIdentity>]
 [-CreatedDateTime <DateTime>] [-Id <String>] [-InternetMessageId <String>] [-OriginalCategory <String>]
 [-ReceivedDateTime <DateTime>] [-RecipientEmailAddress <String>]
 [-Result <IMicrosoftGraphSecuritySubmissionResult>] [-Sender <String>] [-SenderIP <String>] [-Source <String>]
 [-Status <String>] [-Subject <String>]
 [-TenantAllowOrBlockListAction <IMicrosoftGraphSecurityTenantAllowOrBlockListAction>] [-TenantId <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaSecurityThreatSubmissionEmailThreat -EmailThreatSubmissionId <String>
 -BodyParameter <IMicrosoftGraphSecurityEmailThreatSubmission> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaSecurityThreatSubmissionEmailThreat -InputObject <ISecurityIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AdminReview <IMicrosoftGraphSecuritySubmissionAdminReview>]
 [-AttackSimulationInfo <IMicrosoftGraphSecurityAttackSimulationInfo>] [-Category <String>]
 [-ClientSource <String>] [-ContentType <String>] [-CreatedBy <IMicrosoftGraphSecuritySubmissionUserIdentity>]
 [-CreatedDateTime <DateTime>] [-Id <String>] [-InternetMessageId <String>] [-OriginalCategory <String>]
 [-ReceivedDateTime <DateTime>] [-RecipientEmailAddress <String>]
 [-Result <IMicrosoftGraphSecuritySubmissionResult>] [-Sender <String>] [-SenderIP <String>] [-Source <String>]
 [-Status <String>] [-Subject <String>]
 [-TenantAllowOrBlockListAction <IMicrosoftGraphSecurityTenantAllowOrBlockListAction>] [-TenantId <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaSecurityThreatSubmissionEmailThreat -InputObject <ISecurityIdentity>
 -BodyParameter <IMicrosoftGraphSecurityEmailThreatSubmission> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property emailThreats in security

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

### -AdminReview
submissionAdminReview
To construct, see NOTES section for ADMINREVIEW properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecuritySubmissionAdminReview
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AttackSimulationInfo
attackSimulationInfo
To construct, see NOTES section for ATTACKSIMULATIONINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityAttackSimulationInfo
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
emailThreatSubmission
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityEmailThreatSubmission
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Category
submissionCategory

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

### -ClientSource
submissionClientSource

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

### -ContentType
submissionContentType

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

### -CreatedBy
submissionUserIdentity
To construct, see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecuritySubmissionUserIdentity
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
Specifies when the threat submission was created.
Supports $filter = createdDateTime ge 2022-01-01T00:00:00Z and createdDateTime lt 2022-01-02T00:00:00Z.

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

### -EmailThreatSubmissionId
The unique identifier of emailThreatSubmission

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
Type: ISecurityIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InternetMessageId
Specifies the internet message ID of the email being submitted.
This information is present in the email header.

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

### -OriginalCategory
submissionCategory

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

### -ReceivedDateTime
Specifies the date and time stamp when the email was received.

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

### -RecipientEmailAddress
Specifies the email address (in smtp format) of the recipient who received the email.

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

### -Result
submissionResult
To construct, see NOTES section for RESULT properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecuritySubmissionResult
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sender
Specifies the email address of the sender.

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

### -SenderIP
Specifies the IP address of the sender.

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

### -Source
submissionSource

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

### -Status
longRunningOperationStatus

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

### -Subject
Specifies the subject of the email.

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

### -TenantAllowOrBlockListAction
tenantAllowOrBlockListAction
To construct, see NOTES section for TENANTALLOWORBLOCKLISTACTION properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityTenantAllowOrBlockListAction
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TenantId
Indicates the tenant id of the submitter.
Not required when created using a POST operation.
It's extracted from the token of the post API call.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSecurityEmailThreatSubmission
### Microsoft.Graph.Beta.PowerShell.Models.ISecurityIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSecurityEmailThreatSubmission
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ADMINREVIEW `<IMicrosoftGraphSecuritySubmissionAdminReview>`: submissionAdminReview
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ReviewBy <String>]`: Specifies who reviewed the email.
The identification is an email ID or other identity strings.
  - `[ReviewDateTime <DateTime?>]`: Specifies the date time when the review occurred.
  - `[ReviewResult <String>]`: submissionResultCategory

ATTACKSIMULATIONINFO `<IMicrosoftGraphSecurityAttackSimulationInfo>`: attackSimulationInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AttackSimDateTime <DateTime?>]`: The date and time of the attack simulation.
  - `[AttackSimDurationTime <TimeSpan?>]`: The duration (in time) for the attack simulation.
  - `[AttackSimId <String>]`: The activity ID for the attack simulation.
  - `[AttackSimUserId <String>]`: The unique identifier for the user who got the attack simulation email.

BODYPARAMETER `<IMicrosoftGraphSecurityEmailThreatSubmission>`: emailThreatSubmission
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AdminReview <IMicrosoftGraphSecuritySubmissionAdminReview>]`: submissionAdminReview
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ReviewBy <String>]`: Specifies who reviewed the email.
The identification is an email ID or other identity strings.
    - `[ReviewDateTime <DateTime?>]`: Specifies the date time when the review occurred.
    - `[ReviewResult <String>]`: submissionResultCategory
  - `[Category <String>]`: submissionCategory
  - `[ClientSource <String>]`: submissionClientSource
  - `[ContentType <String>]`: submissionContentType
  - `[CreatedBy <IMicrosoftGraphSecuritySubmissionUserIdentity>]`: submissionUserIdentity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
    - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[Email <String>]`: The email of user who is making the submission when logged in (delegated token case).
  - `[CreatedDateTime <DateTime?>]`: Specifies when the threat submission was created.
Supports $filter = createdDateTime ge 2022-01-01T00:00:00Z and createdDateTime lt 2022-01-02T00:00:00Z.
  - `[Result <IMicrosoftGraphSecuritySubmissionResult>]`: submissionResult
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Category <String>]`: submissionResultCategory
    - `[Detail <String>]`: submissionResultDetail
    - `[DetectedFiles <IMicrosoftGraphSecuritySubmissionDetectedFile- `[]`>]`: Specifies the files detected by Microsoft in the submitted emails.
      - `[FileHash <String>]`: The file hash.
      - `[FileName <String>]`: The file name.
    - `[DetectedUrls <String- `[]`>]`: Specifies the URLs detected by Microsoft in the submitted email.
    - `[UserMailboxSetting <String>]`: userMailboxSetting
  - `[Source <String>]`: submissionSource
  - `[Status <String>]`: longRunningOperationStatus
  - `[TenantId <String>]`: Indicates the tenant id of the submitter.
Not required when created using a POST operation.
It's extracted from the token of the post API call.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AttackSimulationInfo <IMicrosoftGraphSecurityAttackSimulationInfo>]`: attackSimulationInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AttackSimDateTime <DateTime?>]`: The date and time of the attack simulation.
    - `[AttackSimDurationTime <TimeSpan?>]`: The duration (in time) for the attack simulation.
    - `[AttackSimId <String>]`: The activity ID for the attack simulation.
    - `[AttackSimUserId <String>]`: The unique identifier for the user who got the attack simulation email.
  - `[InternetMessageId <String>]`: Specifies the internet message ID of the email being submitted.
This information is present in the email header.
  - `[OriginalCategory <String>]`: submissionCategory
  - `[ReceivedDateTime <DateTime?>]`: Specifies the date and time stamp when the email was received.
  - `[RecipientEmailAddress <String>]`: Specifies the email address (in smtp format) of the recipient who received the email.
  - `[Sender <String>]`: Specifies the email address of the sender.
  - `[SenderIP <String>]`: Specifies the IP address of the sender.
  - `[Subject <String>]`: Specifies the subject of the email.
  - `[TenantAllowOrBlockListAction <IMicrosoftGraphSecurityTenantAllowOrBlockListAction>]`: tenantAllowOrBlockListAction
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Action <String>]`: tenantAllowBlockListAction
    - `[ExpirationDateTime <DateTime?>]`: Specifies when the tenant allow-block-list expires in date time.
    - `[Note <String>]`: Specifies the note added to the tenant allow-or-block list entry in the format of string.
    - `[Results <IMicrosoftGraphSecurityTenantAllowBlockListEntryResult- `[]`>]`: Contains the result of the submission that lead to the tenant allow-block-list entry creation.
      - `[EntryType <String>]`: tenantAllowBlockListEntryType
      - `[ExpirationDateTime <DateTime?>]`: Specifies the date and time when the entry expires.
      - `[Identity <String>]`: Specifies the identity of the entry generated by the tenant allow block list system.
      - `[Status <String>]`: longRunningOperationStatus
      - `[Value <String>]`: Specifies the value of the created tenant allow block list entry.

CREATEDBY `<IMicrosoftGraphSecuritySubmissionUserIdentity>`: submissionUserIdentity
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
  - `[Id <String>]`: The identifier of the identity.
This property is read-only.
  - `[Email <String>]`: The email of user who is making the submission when logged in (delegated token case).

INPUTOBJECT `<ISecurityIdentity>`: Identity Parameter
  - `[AlertId <String>]`: The unique identifier of alert
  - `[AnalyzedEmailId <String>]`: The unique identifier of analyzedEmail
  - `[ArticleId <String>]`: The unique identifier of article
  - `[ArticleIndicatorId <String>]`: The unique identifier of articleIndicator
  - `[AttackSimulationOperationId <String>]`: The unique identifier of attackSimulationOperation
  - `[AuditLogQueryId <String>]`: The unique identifier of auditLogQuery
  - `[AuditLogRecordId <String>]`: The unique identifier of auditLogRecord
  - `[AuthoredNoteId <String>]`: The unique identifier of authoredNote
  - `[AuthorityTemplateId <String>]`: The unique identifier of authorityTemplate
  - `[CaseOperationId <String>]`: The unique identifier of caseOperation
  - `[CategoryTemplateId <String>]`: The unique identifier of categoryTemplate
  - `[CitationTemplateId <String>]`: The unique identifier of citationTemplate
  - `[CloudAppDiscoveryReportId <String>]`: The unique identifier of cloudAppDiscoveryReport
  - `[CloudAppSecurityProfileId <String>]`: The unique identifier of cloudAppSecurityProfile
  - `[CustomerInsightTenantId <String>]`: The unique identifier of customerInsight
  - `[DataSourceId <String>]`: The unique identifier of dataSource
  - `[DepartmentTemplateId <String>]`: The unique identifier of departmentTemplate
  - `[DetectionRuleId <String>]`: The unique identifier of detectionRule
  - `[DispositionReviewStageNumber <String>]`: The unique identifier of dispositionReviewStage
  - `[DomainSecurityProfileId <String>]`: The unique identifier of domainSecurityProfile
  - `[EdiscoveryCaseId <String>]`: The unique identifier of ediscoveryCase
  - `[EdiscoveryCaseMemberId <String>]`: The unique identifier of ediscoveryCaseMember
  - `[EdiscoveryCustodianId <String>]`: The unique identifier of ediscoveryCustodian
  - `[EdiscoveryFileId <String>]`: The unique identifier of ediscoveryFile
  - `[EdiscoveryHoldPolicyId <String>]`: The unique identifier of ediscoveryHoldPolicy
  - `[EdiscoveryNoncustodialDataSourceId <String>]`: The unique identifier of ediscoveryNoncustodialDataSource
  - `[EdiscoveryReviewSetId <String>]`: The unique identifier of ediscoveryReviewSet
  - `[EdiscoveryReviewSetQueryId <String>]`: The unique identifier of ediscoveryReviewSetQuery
  - `[EdiscoveryReviewTagId <String>]`: The unique identifier of ediscoveryReviewTag
  - `[EdiscoveryReviewTagId1 <String>]`: The unique identifier of ediscoveryReviewTag
  - `[EdiscoverySearchId <String>]`: The unique identifier of ediscoverySearch
  - `[EmailThreatSubmissionId <String>]`: The unique identifier of emailThreatSubmission
  - `[EmailThreatSubmissionPolicyId <String>]`: The unique identifier of emailThreatSubmissionPolicy
  - `[EndUserNotificationDetailId <String>]`: The unique identifier of endUserNotificationDetail
  - `[EndUserNotificationId <String>]`: The unique identifier of endUserNotification
  - `[FilePlanReferenceTemplateId <String>]`: The unique identifier of filePlanReferenceTemplate
  - `[FileSecurityProfileId <String>]`: The unique identifier of fileSecurityProfile
  - `[FileThreatSubmissionId <String>]`: The unique identifier of fileThreatSubmission
  - `[HealthIssueId <String>]`: The unique identifier of healthIssue
  - `[HostComponentId <String>]`: The unique identifier of hostComponent
  - `[HostCookieId <String>]`: The unique identifier of hostCookie
  - `[HostId <String>]`: The unique identifier of host
  - `[HostPairId <String>]`: The unique identifier of hostPair
  - `[HostPortId <String>]`: The unique identifier of hostPort
  - `[HostSecurityProfileId <String>]`: The unique identifier of hostSecurityProfile
  - `[HostSslCertificateId <String>]`: The unique identifier of hostSslCertificate
  - `[HostTrackerId <String>]`: The unique identifier of hostTracker
  - `[IPSecurityProfileId <String>]`: The unique identifier of ipSecurityProfile
  - `[IncidentId <String>]`: The unique identifier of incident
  - `[IntelligenceProfileId <String>]`: The unique identifier of intelligenceProfile
  - `[IntelligenceProfileIndicatorId <String>]`: The unique identifier of intelligenceProfileIndicator
  - `[LandingPageDetailId <String>]`: The unique identifier of landingPageDetail
  - `[LandingPageId <String>]`: The unique identifier of landingPage
  - `[LoginPageId <String>]`: The unique identifier of loginPage
  - `[PartnerSecurityAlertId <String>]`: The unique identifier of partnerSecurityAlert
  - `[PassiveDnsRecordId <String>]`: The unique identifier of passiveDnsRecord
  - `[PayloadId <String>]`: The unique identifier of payload
  - `[ProviderTenantSettingId <String>]`: The unique identifier of providerTenantSetting
  - `[RetentionEventId <String>]`: The unique identifier of retentionEvent
  - `[RetentionEventTypeId <String>]`: The unique identifier of retentionEventType
  - `[RetentionLabelId <String>]`: The unique identifier of retentionLabel
  - `[SecureScoreControlProfileId <String>]`: The unique identifier of secureScoreControlProfile
  - `[SecureScoreId <String>]`: The unique identifier of secureScore
  - `[SecurityActionId <String>]`: The unique identifier of securityAction
  - `[SecurityRequirementId <String>]`: The unique identifier of securityRequirement
  - `[SecurityScoreHistoryId <String>]`: The unique identifier of securityScoreHistory
  - `[SensitivityLabelId <String>]`: The unique identifier of sensitivityLabel
  - `[SensorId <String>]`: The unique identifier of sensor
  - `[SimulationAutomationId <String>]`: The unique identifier of simulationAutomation
  - `[SimulationAutomationRunId <String>]`: The unique identifier of simulationAutomationRun
  - `[SimulationId <String>]`: The unique identifier of simulation
  - `[SiteSourceId <String>]`: The unique identifier of siteSource
  - `[SslCertificateId <String>]`: The unique identifier of sslCertificate
  - `[SubcategoryTemplateId <String>]`: The unique identifier of subcategoryTemplate
  - `[SubdomainId <String>]`: The unique identifier of subdomain
  - `[SubjectRightsRequestId <String>]`: The unique identifier of subjectRightsRequest
  - `[TiIndicatorId <String>]`: The unique identifier of tiIndicator
  - `[TrainingCampaignId <String>]`: The unique identifier of trainingCampaign
  - `[TrainingId <String>]`: The unique identifier of training
  - `[TrainingLanguageDetailId <String>]`: The unique identifier of trainingLanguageDetail
  - `[UnifiedGroupSourceId <String>]`: The unique identifier of unifiedGroupSource
  - `[UrlThreatSubmissionId <String>]`: The unique identifier of urlThreatSubmission
  - `[UserId <String>]`: The unique identifier of user
  - `[UserPrincipalName <String>]`: Alternate key of user
  - `[UserSecurityProfileId <String>]`: The unique identifier of userSecurityProfile
  - `[UserSourceId <String>]`: The unique identifier of userSource
  - `[VulnerabilityComponentId <String>]`: The unique identifier of vulnerabilityComponent
  - `[VulnerabilityId <String>]`: The unique identifier of vulnerability
  - `[WhoisHistoryRecordId <String>]`: The unique identifier of whoisHistoryRecord
  - `[WhoisRecordId <String>]`: The unique identifier of whoisRecord

RESULT `<IMicrosoftGraphSecuritySubmissionResult>`: submissionResult
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Category <String>]`: submissionResultCategory
  - `[Detail <String>]`: submissionResultDetail
  - `[DetectedFiles <IMicrosoftGraphSecuritySubmissionDetectedFile- `[]`>]`: Specifies the files detected by Microsoft in the submitted emails.
    - `[FileHash <String>]`: The file hash.
    - `[FileName <String>]`: The file name.
  - `[DetectedUrls <String- `[]`>]`: Specifies the URLs detected by Microsoft in the submitted email.
  - `[UserMailboxSetting <String>]`: userMailboxSetting

TENANTALLOWORBLOCKLISTACTION `<IMicrosoftGraphSecurityTenantAllowOrBlockListAction>`: tenantAllowOrBlockListAction
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Action <String>]`: tenantAllowBlockListAction
  - `[ExpirationDateTime <DateTime?>]`: Specifies when the tenant allow-block-list expires in date time.
  - `[Note <String>]`: Specifies the note added to the tenant allow-or-block list entry in the format of string.
  - `[Results <IMicrosoftGraphSecurityTenantAllowBlockListEntryResult- `[]`>]`: Contains the result of the submission that lead to the tenant allow-block-list entry creation.
    - `[EntryType <String>]`: tenantAllowBlockListEntryType
    - `[ExpirationDateTime <DateTime?>]`: Specifies the date and time when the entry expires.
    - `[Identity <String>]`: Specifies the identity of the entry generated by the tenant allow block list system.
    - `[Status <String>]`: longRunningOperationStatus
    - `[Value <String>]`: Specifies the value of the created tenant allow block list entry.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/update-mgbetasecuritythreatsubmissionemailthreat](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/update-mgbetasecuritythreatsubmissionemailthreat)
























