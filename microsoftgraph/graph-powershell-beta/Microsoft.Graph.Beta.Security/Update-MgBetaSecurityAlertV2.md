---
external help file: Microsoft.Graph.Beta.Security-help.xml
Module Name: Microsoft.Graph.Beta.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/update-mgbetasecurityalertv2
schema: 2.0.0
ms.subservice: security
---

# Update-MgBetaSecurityAlertV2

## SYNOPSIS
Update the properties of an alert object.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgSecurityAlertV2](/powershell/module/Microsoft.Graph.Security/Update-MgSecurityAlertV2?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaSecurityAlertV2 -AlertId <String> [-ResponseHeadersVariable <String>] [-ActorDisplayName <String>]
 [-AdditionalData <Hashtable>] [-AdditionalProperties <Hashtable>] [-AlertPolicyId <String>]
 [-AlertWebUrl <String>] [-AssignedTo <String>] [-Category <String>] [-Classification <String>]
 [-Comments <IMicrosoftGraphSecurityAlertComment[]>] [-CreatedDateTime <DateTime>] [-Description <String>]
 [-DetectionSource <String>] [-DetectorId <String>] [-Determination <String>]
 [-Evidence <IMicrosoftGraphSecurityAlertEvidence[]>] [-FirstActivityDateTime <DateTime>] [-Id <String>]
 [-IncidentId <String>] [-IncidentWebUrl <String>] [-LastActivityDateTime <DateTime>]
 [-LastUpdateDateTime <DateTime>] [-MitreTechniques <String[]>] [-ProductName <String>]
 [-ProviderAlertId <String>] [-RecommendedActions <String>] [-ResolvedDateTime <DateTime>]
 [-ServiceSource <String>] [-Severity <String>] [-Status <String>] [-SystemTags <String[]>]
 [-TenantId <String>] [-ThreatDisplayName <String>] [-ThreatFamilyName <String>] [-Title <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaSecurityAlertV2 -AlertId <String> -BodyParameter <IMicrosoftGraphSecurityAlert>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaSecurityAlertV2 -InputObject <ISecurityIdentity> [-ResponseHeadersVariable <String>]
 [-ActorDisplayName <String>] [-AdditionalData <Hashtable>] [-AdditionalProperties <Hashtable>]
 [-AlertPolicyId <String>] [-AlertWebUrl <String>] [-AssignedTo <String>] [-Category <String>]
 [-Classification <String>] [-Comments <IMicrosoftGraphSecurityAlertComment[]>] [-CreatedDateTime <DateTime>]
 [-Description <String>] [-DetectionSource <String>] [-DetectorId <String>] [-Determination <String>]
 [-Evidence <IMicrosoftGraphSecurityAlertEvidence[]>] [-FirstActivityDateTime <DateTime>] [-Id <String>]
 [-IncidentId <String>] [-IncidentWebUrl <String>] [-LastActivityDateTime <DateTime>]
 [-LastUpdateDateTime <DateTime>] [-MitreTechniques <String[]>] [-ProductName <String>]
 [-ProviderAlertId <String>] [-RecommendedActions <String>] [-ResolvedDateTime <DateTime>]
 [-ServiceSource <String>] [-Severity <String>] [-Status <String>] [-SystemTags <String[]>]
 [-TenantId <String>] [-ThreatDisplayName <String>] [-ThreatFamilyName <String>] [-Title <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaSecurityAlertV2 -InputObject <ISecurityIdentity> -BodyParameter <IMicrosoftGraphSecurityAlert>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of an alert object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | SecurityAlert.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | SecurityAlert.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	assignedTo = "secAdmin@contoso.com"
	classification = "truePositive"
	determination = "malware"
	status = "inProgress"
}

Update-MgBetaSecurityAlertV2 -AlertId $alertId -BodyParameter $params

```
This example shows how to use the Update-MgBetaSecurityAlertV2 Cmdlet.


## PARAMETERS

### -ActorDisplayName
The adversary or activity group that is associated with this alert.

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

### -AdditionalData
dictionary

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

### -AlertId
The unique identifier of alert

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

### -AlertPolicyId
The ID of the policy that generated the alert, and populated when there is a specific policy that generated the alert, whether configured by a customer or a built-in policy.

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

### -AlertWebUrl
URL for the Microsoft 365 Defender portal alert page.

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

### -AssignedTo
Owner of the alert, or null if no owner is assigned.

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
alert
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityAlert
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Category
The attack kill-chain category that the alert belongs to.
Aligned with the MITRE ATT&CK framework.

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

### -Classification
alertClassification

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

### -Comments
Array of comments created by the Security Operations (SecOps) team during the alert management process.
To construct, see NOTES section for COMMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityAlertComment[]
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

### -CreatedDateTime
Time when Microsoft 365 Defender created the alert.

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

### -Description
String value describing each alert.

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

### -DetectionSource
detectionSource

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

### -DetectorId
The ID of the detector that triggered the alert.

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

### -Determination
alertDetermination

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

### -Evidence
Collection of evidence related to the alert.
To construct, see NOTES section for EVIDENCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityAlertEvidence[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FirstActivityDateTime
The earliest activity associated with the alert.

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

### -IncidentId
Unique identifier to represent the incident this alert resource is associated with.

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

### -IncidentWebUrl
URL for the incident page in the Microsoft 365 Defender portal.

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

### -LastActivityDateTime
The oldest activity associated with the alert.

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

### -LastUpdateDateTime
Time when the alert was last updated at Microsoft 365 Defender.

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

### -MitreTechniques
The attack techniques, as aligned with the MITRE ATT&CK framework.

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

### -ProductName
The name of the product which published this alert.

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

### -ProviderAlertId
The ID of the alert as it appears in the security provider product that generated the alert.

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

### -RecommendedActions
Recommended response and remediation actions to take in the event this alert was generated.

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

### -ResolvedDateTime
Time when the alert was resolved.

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

### -ServiceSource
serviceSource

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

### -Severity
alertSeverity

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
alertStatus

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

### -SystemTags
The system tags associated with the alert.

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

### -TenantId
The Microsoft Entra tenant the alert was created in.

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

### -ThreatDisplayName
The threat associated with this alert.

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

### -ThreatFamilyName
Threat family associated with this alert.

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

### -Title
Brief identifying string value describing the alert.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSecurityAlert
### Microsoft.Graph.Beta.PowerShell.Models.ISecurityIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSecurityAlert
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphSecurityAlert>`: alert
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActorDisplayName <String>]`: The adversary or activity group that is associated with this alert.
  - `[AdditionalData <IMicrosoftGraphSecurityDictionary>]`: dictionary
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AlertPolicyId <String>]`: The ID of the policy that generated the alert, and populated when there is a specific policy that generated the alert, whether configured by a customer or a built-in policy.
  - `[AlertWebUrl <String>]`: URL for the Microsoft 365 Defender portal alert page.
  - `[AssignedTo <String>]`: Owner of the alert, or null if no owner is assigned.
  - `[Category <String>]`: The attack kill-chain category that the alert belongs to.
Aligned with the MITRE ATT&CK framework.
  - `[Classification <String>]`: alertClassification
  - `[Comments <IMicrosoftGraphSecurityAlertComment- `[]`>]`: Array of comments created by the Security Operations (SecOps) team during the alert management process.
    - `[Comment <String>]`: The comment text.
    - `[CreatedByDisplayName <String>]`: The person or app name that submitted the comment.
    - `[CreatedDateTime <DateTime?>]`: The time when the comment was submitted.
  - `[CreatedDateTime <DateTime?>]`: Time when Microsoft 365 Defender created the alert.
  - `[Description <String>]`: String value describing each alert.
  - `[DetectionSource <String>]`: detectionSource
  - `[DetectorId <String>]`: The ID of the detector that triggered the alert.
  - `[Determination <String>]`: alertDetermination
  - `[Evidence <IMicrosoftGraphSecurityAlertEvidence- `[]`>]`: Collection of evidence related to the alert.
    - `[CreatedDateTime <DateTime?>]`: The date and time when the evidence was created and added to the alert.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[DetailedRoles <String- `[]`>]`: Detailed description of the entity role/s in an alert.
Values are free-form.
    - `[RemediationStatus <String>]`: evidenceRemediationStatus
    - `[RemediationStatusDetails <String>]`: Details about the remediation status.
    - `[Roles <String- `[]`>]`: The role/s that an evidence entity represents in an alert, for example, an IP address that is associated with an attacker has the evidence role Attacker.
    - `[Tags <String- `[]`>]`: Array of custom tags associated with an evidence instance, for example, to denote a group of devices, high-value assets, etc.
    - `[Verdict <String>]`: evidenceVerdict
  - `[FirstActivityDateTime <DateTime?>]`: The earliest activity associated with the alert.
  - `[IncidentId <String>]`: Unique identifier to represent the incident this alert resource is associated with.
  - `[IncidentWebUrl <String>]`: URL for the incident page in the Microsoft 365 Defender portal.
  - `[LastActivityDateTime <DateTime?>]`: The oldest activity associated with the alert.
  - `[LastUpdateDateTime <DateTime?>]`: Time when the alert was last updated at Microsoft 365 Defender.
  - `[MitreTechniques <String- `[]`>]`: The attack techniques, as aligned with the MITRE ATT&CK framework.
  - `[ProductName <String>]`: The name of the product which published this alert.
  - `[ProviderAlertId <String>]`: The ID of the alert as it appears in the security provider product that generated the alert.
  - `[RecommendedActions <String>]`: Recommended response and remediation actions to take in the event this alert was generated.
  - `[ResolvedDateTime <DateTime?>]`: Time when the alert was resolved.
  - `[ServiceSource <String>]`: serviceSource
  - `[Severity <String>]`: alertSeverity
  - `[Status <String>]`: alertStatus
  - `[SystemTags <String- `[]`>]`: The system tags associated with the alert.
  - `[TenantId <String>]`: The Microsoft Entra tenant the alert was created in.
  - `[ThreatDisplayName <String>]`: The threat associated with this alert.
  - `[ThreatFamilyName <String>]`: Threat family associated with this alert.
  - `[Title <String>]`: Brief identifying string value describing the alert.

COMMENTS `<IMicrosoftGraphSecurityAlertComment- `[]`>`: Array of comments created by the Security Operations (SecOps) team during the alert management process.
  - `[Comment <String>]`: The comment text.
  - `[CreatedByDisplayName <String>]`: The person or app name that submitted the comment.
  - `[CreatedDateTime <DateTime?>]`: The time when the comment was submitted.

EVIDENCE `<IMicrosoftGraphSecurityAlertEvidence- `[]`>`: Collection of evidence related to the alert.
  - `[CreatedDateTime <DateTime?>]`: The date and time when the evidence was created and added to the alert.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[DetailedRoles <String- `[]`>]`: Detailed description of the entity role/s in an alert.
Values are free-form.
  - `[RemediationStatus <String>]`: evidenceRemediationStatus
  - `[RemediationStatusDetails <String>]`: Details about the remediation status.
  - `[Roles <String- `[]`>]`: The role/s that an evidence entity represents in an alert, for example, an IP address that is associated with an attacker has the evidence role Attacker.
  - `[Tags <String- `[]`>]`: Array of custom tags associated with an evidence instance, for example, to denote a group of devices, high-value assets, etc.
  - `[Verdict <String>]`: evidenceVerdict

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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/update-mgbetasecurityalertv2](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/update-mgbetasecurityalertv2)

[https://learn.microsoft.com/graph/api/security-alert-update?view=graph-rest-beta](https://learn.microsoft.com/graph/api/security-alert-update?view=graph-rest-beta)























