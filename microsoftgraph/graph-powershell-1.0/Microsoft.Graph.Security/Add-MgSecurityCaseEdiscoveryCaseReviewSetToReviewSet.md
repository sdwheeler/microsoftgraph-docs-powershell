---
external help file: Microsoft.Graph.Security-help.xml
Module Name: Microsoft.Graph.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.security/add-mgsecuritycaseediscoverycasereviewsettoreviewset
schema: 2.0.0
ms.subservice: ediscovery
---

# Add-MgSecurityCaseEdiscoveryCaseReviewSetToReviewSet

## SYNOPSIS
Start the process of adding a collection from Microsoft 365 services to a review set.
After the operation is created, you can get the status of the operation by retrieving the Location parameter from the response headers.
The location provides a URL that will return a Add to review set operation.

> [!NOTE]
> To view the beta release of this cmdlet, view [Add-MgBetaSecurityCaseEdiscoveryCaseReviewSetToReviewSet](/powershell/module/Microsoft.Graph.Beta.Security/Add-MgBetaSecurityCaseEdiscoveryCaseReviewSetToReviewSet?view=graph-powershell-beta)

## SYNTAX

### AddExpanded (Default)
```
Add-MgSecurityCaseEdiscoveryCaseReviewSetToReviewSet -EdiscoveryCaseId <String> -EdiscoveryReviewSetId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalDataOptions <String>] [-AdditionalProperties <Hashtable>]
 [-CloudAttachmentVersion <String>] [-DocumentVersion <String>] [-ItemsToInclude <String>]
 [-Search <IMicrosoftGraphSecurityEdiscoverySearch>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Add
```
Add-MgSecurityCaseEdiscoveryCaseReviewSetToReviewSet -EdiscoveryCaseId <String> -EdiscoveryReviewSetId <String>
 -BodyParameter <IPathsZszldxSecurityCasesEdiscoverycasesEdiscoverycaseIdReviewsetsEdiscoveryreviewsetIdMicrosoftGraphSecurityAddtoreviewsetPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### AddViaIdentityExpanded
```
Add-MgSecurityCaseEdiscoveryCaseReviewSetToReviewSet -InputObject <ISecurityIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalDataOptions <String>] [-AdditionalProperties <Hashtable>]
 [-CloudAttachmentVersion <String>] [-DocumentVersion <String>] [-ItemsToInclude <String>]
 [-Search <IMicrosoftGraphSecurityEdiscoverySearch>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### AddViaIdentity
```
Add-MgSecurityCaseEdiscoveryCaseReviewSetToReviewSet -InputObject <ISecurityIdentity>
 -BodyParameter <IPathsZszldxSecurityCasesEdiscoverycasesEdiscoverycaseIdReviewsetsEdiscoveryreviewsetIdMicrosoftGraphSecurityAddtoreviewsetPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Start the process of adding a collection from Microsoft 365 services to a review set.
After the operation is created, you can get the status of the operation by retrieving the Location parameter from the response headers.
The location provides a URL that will return a Add to review set operation.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | eDiscovery.Read.All, eDiscovery.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | eDiscovery.Read.All, eDiscovery.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Security

$params = @{
	search = @{
		id = "c17e91d6-6bc0-4ecb-b388-269ea3d4ffb7"
	}
	additionalDataOptions = "linkedFiles"
}

Add-MgSecurityCaseEdiscoveryCaseReviewSetToReviewSet -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryReviewSetId $ediscoveryReviewSetId -BodyParameter $params

```
This example shows how to use the Add-MgSecurityCaseEdiscoveryCaseReviewSetToReviewSet Cmdlet.


## PARAMETERS

### -AdditionalDataOptions
additionalDataOptions

```yaml
Type: String
Parameter Sets: AddExpanded, AddViaIdentityExpanded
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
Parameter Sets: AddExpanded, AddViaIdentityExpanded
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
Type: IPathsZszldxSecurityCasesEdiscoverycasesEdiscoverycaseIdReviewsetsEdiscoveryreviewsetIdMicrosoftGraphSecurityAddtoreviewsetPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Add, AddViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CloudAttachmentVersion
cloudAttachmentVersion

```yaml
Type: String
Parameter Sets: AddExpanded, AddViaIdentityExpanded
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

### -DocumentVersion
documentVersion

```yaml
Type: String
Parameter Sets: AddExpanded, AddViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EdiscoveryCaseId
The unique identifier of ediscoveryCase

```yaml
Type: String
Parameter Sets: AddExpanded, Add
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EdiscoveryReviewSetId
The unique identifier of ediscoveryReviewSet

```yaml
Type: String
Parameter Sets: AddExpanded, Add
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ISecurityIdentity
Parameter Sets: AddViaIdentityExpanded, AddViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ItemsToInclude
itemsToInclude

```yaml
Type: String
Parameter Sets: AddExpanded, AddViaIdentityExpanded
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

### -Search
ediscoverySearch
To construct, see NOTES section for SEARCH properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityEdiscoverySearch
Parameter Sets: AddExpanded, AddViaIdentityExpanded
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

### Microsoft.Graph.PowerShell.Models.IPathsZszldxSecurityCasesEdiscoverycasesEdiscoverycaseIdReviewsetsEdiscoveryreviewsetIdMicrosoftGraphSecurityAddtoreviewsetPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.PowerShell.Models.ISecurityIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsZszldxSecurityCasesEdiscoverycasesEdiscoverycaseIdReviewsetsEdiscoveryreviewsetIdMicrosoftGraphSecurityAddtoreviewsetPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AdditionalDataOptions <String>]`: additionalDataOptions
  - `[CloudAttachmentVersion <String>]`: cloudAttachmentVersion
  - `[DocumentVersion <String>]`: documentVersion
  - `[ItemsToInclude <String>]`: itemsToInclude
  - `[Search <IMicrosoftGraphSecurityEdiscoverySearch>]`: ediscoverySearch
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ContentQuery <String>]`:
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[CreatedDateTime <DateTime?>]`:
    - `[Description <String>]`:
    - `[DisplayName <String>]`:
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedDateTime <DateTime?>]`:
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AddToReviewSetOperation <IMicrosoftGraphSecurityEdiscoveryAddToReviewSetOperation>]`: ediscoveryAddToReviewSetOperation
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Action <String>]`: caseAction
      - `[CompletedDateTime <DateTime?>]`: The date and time the operation was completed.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: The date and time the operation was created.
      - `[PercentProgress <Int32?>]`: The progress of the operation.
      - `[ResultInfo <IMicrosoftGraphResultInfo>]`: resultInfo
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Code <Int32?>]`: The result code.
        - `[Message <String>]`: The message.
        - `[Subcode <Int32?>]`: The result subcode.
      - `[Status <String>]`: caseOperationStatus
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AdditionalDataOptions <String>]`: additionalDataOptions
      - `[CloudAttachmentVersion <String>]`: cloudAttachmentVersion
      - `[DocumentVersion <String>]`: documentVersion
      - `[ItemsToInclude <String>]`: itemsToInclude
      - `[ReviewSet <IMicrosoftGraphSecurityEdiscoveryReviewSet>]`: ediscoveryReviewSet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[CreatedDateTime <DateTime?>]`:
        - `[Description <String>]`:
        - `[DisplayName <String>]`:
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[Queries <IMicrosoftGraphSecurityEdiscoveryReviewSetQuery- `[]`>]`: Represents queries within the review set.
          - `[ContentQuery <String>]`:
          - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
          - `[CreatedDateTime <DateTime?>]`:
          - `[Description <String>]`:
          - `[DisplayName <String>]`:
          - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
          - `[LastModifiedDateTime <DateTime?>]`:
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Search <IMicrosoftGraphSecurityEdiscoverySearch>]`: ediscoverySearch
    - `[AdditionalSources <IMicrosoftGraphSecurityDataSource- `[]`>]`: Adds an additional source to the eDiscovery search.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: The date and time the dataSource was created.
      - `[DisplayName <String>]`: The display name of the dataSource and is the name of the SharePoint site.
      - `[HoldStatus <String>]`: dataSourceHoldStatus
    - `[CustodianSources <IMicrosoftGraphSecurityDataSource- `[]`>]`: Custodian sources that are included in the eDiscovery search.
    - `[DataSourceScopes <String>]`: dataSourceScopes
    - `[LastEstimateStatisticsOperation <IMicrosoftGraphSecurityEdiscoveryEstimateOperation>]`: ediscoveryEstimateOperation
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Action <String>]`: caseAction
      - `[CompletedDateTime <DateTime?>]`: The date and time the operation was completed.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: The date and time the operation was created.
      - `[PercentProgress <Int32?>]`: The progress of the operation.
      - `[ResultInfo <IMicrosoftGraphResultInfo>]`: resultInfo
      - `[Status <String>]`: caseOperationStatus
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[IndexedItemCount <Int64?>]`: The estimated count of items for the search that matched the content query.
      - `[IndexedItemsSize <Int64?>]`: The estimated size of items for the search that matched the content query.
      - `[MailboxCount <Int32?>]`: The number of mailboxes that had search hits.
      - `[Search <IMicrosoftGraphSecurityEdiscoverySearch>]`: ediscoverySearch
      - `[SiteCount <Int32?>]`: The number of mailboxes that had search hits.
      - `[StatisticsOptions <String>]`: statisticsOptions
      - `[UnindexedItemCount <Int64?>]`: The estimated count of unindexed items for the collection.
      - `[UnindexedItemsSize <Int64?>]`: The estimated size of unindexed items for the collection.
    - `[NoncustodialSources <IMicrosoftGraphSecurityEdiscoveryNoncustodialDataSource- `[]`>]`: noncustodialDataSource sources that are included in the eDiscovery search
      - `[CreatedDateTime <DateTime?>]`: Created date and time of the dataSourceContainer entity.
      - `[DisplayName <String>]`: Display name of the dataSourceContainer entity.
      - `[HoldStatus <String>]`: dataSourceHoldStatus
      - `[LastModifiedDateTime <DateTime?>]`: Last modified date and time of the dataSourceContainer.
      - `[ReleasedDateTime <DateTime?>]`: Date and time that the dataSourceContainer was released from the case.
      - `[Status <String>]`: dataSourceContainerStatus
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DataSource <IMicrosoftGraphSecurityDataSource>]`: dataSource
      - `[LastIndexOperation <IMicrosoftGraphSecurityEdiscoveryIndexOperation>]`: ediscoveryIndexOperation
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Action <String>]`: caseAction
        - `[CompletedDateTime <DateTime?>]`: The date and time the operation was completed.
        - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[CreatedDateTime <DateTime?>]`: The date and time the operation was created.
        - `[PercentProgress <Int32?>]`: The progress of the operation.
        - `[ResultInfo <IMicrosoftGraphResultInfo>]`: resultInfo
        - `[Status <String>]`: caseOperationStatus
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.

INPUTOBJECT `<ISecurityIdentity>`: Identity Parameter
  - `[AlertId <String>]`: The unique identifier of alert
  - `[ArticleId <String>]`: The unique identifier of article
  - `[ArticleIndicatorId <String>]`: The unique identifier of articleIndicator
  - `[AttackSimulationOperationId <String>]`: The unique identifier of attackSimulationOperation
  - `[AuthoredNoteId <String>]`: The unique identifier of authoredNote
  - `[AuthorityTemplateId <String>]`: The unique identifier of authorityTemplate
  - `[CaseOperationId <String>]`: The unique identifier of caseOperation
  - `[CategoryTemplateId <String>]`: The unique identifier of categoryTemplate
  - `[CitationTemplateId <String>]`: The unique identifier of citationTemplate
  - `[DataSourceId <String>]`: The unique identifier of dataSource
  - `[DepartmentTemplateId <String>]`: The unique identifier of departmentTemplate
  - `[DispositionReviewStageNumber <String>]`: The unique identifier of dispositionReviewStage
  - `[EdiscoveryCaseId <String>]`: The unique identifier of ediscoveryCase
  - `[EdiscoveryCustodianId <String>]`: The unique identifier of ediscoveryCustodian
  - `[EdiscoveryNoncustodialDataSourceId <String>]`: The unique identifier of ediscoveryNoncustodialDataSource
  - `[EdiscoveryReviewSetId <String>]`: The unique identifier of ediscoveryReviewSet
  - `[EdiscoveryReviewSetQueryId <String>]`: The unique identifier of ediscoveryReviewSetQuery
  - `[EdiscoveryReviewTagId <String>]`: The unique identifier of ediscoveryReviewTag
  - `[EdiscoveryReviewTagId1 <String>]`: The unique identifier of ediscoveryReviewTag
  - `[EdiscoverySearchId <String>]`: The unique identifier of ediscoverySearch
  - `[EndUserNotificationDetailId <String>]`: The unique identifier of endUserNotificationDetail
  - `[EndUserNotificationId <String>]`: The unique identifier of endUserNotification
  - `[FilePlanReferenceTemplateId <String>]`: The unique identifier of filePlanReferenceTemplate
  - `[HealthIssueId <String>]`: The unique identifier of healthIssue
  - `[HostComponentId <String>]`: The unique identifier of hostComponent
  - `[HostCookieId <String>]`: The unique identifier of hostCookie
  - `[HostId <String>]`: The unique identifier of host
  - `[HostPairId <String>]`: The unique identifier of hostPair
  - `[HostPortId <String>]`: The unique identifier of hostPort
  - `[HostSslCertificateId <String>]`: The unique identifier of hostSslCertificate
  - `[HostTrackerId <String>]`: The unique identifier of hostTracker
  - `[IncidentId <String>]`: The unique identifier of incident
  - `[IntelligenceProfileId <String>]`: The unique identifier of intelligenceProfile
  - `[IntelligenceProfileIndicatorId <String>]`: The unique identifier of intelligenceProfileIndicator
  - `[LandingPageDetailId <String>]`: The unique identifier of landingPageDetail
  - `[LandingPageId <String>]`: The unique identifier of landingPage
  - `[LoginPageId <String>]`: The unique identifier of loginPage
  - `[PassiveDnsRecordId <String>]`: The unique identifier of passiveDnsRecord
  - `[PayloadId <String>]`: The unique identifier of payload
  - `[RetentionEventId <String>]`: The unique identifier of retentionEvent
  - `[RetentionEventTypeId <String>]`: The unique identifier of retentionEventType
  - `[RetentionLabelId <String>]`: The unique identifier of retentionLabel
  - `[SecureScoreControlProfileId <String>]`: The unique identifier of secureScoreControlProfile
  - `[SecureScoreId <String>]`: The unique identifier of secureScore
  - `[SensorId <String>]`: The unique identifier of sensor
  - `[SimulationAutomationId <String>]`: The unique identifier of simulationAutomation
  - `[SimulationAutomationRunId <String>]`: The unique identifier of simulationAutomationRun
  - `[SimulationId <String>]`: The unique identifier of simulation
  - `[SiteSourceId <String>]`: The unique identifier of siteSource
  - `[SslCertificateId <String>]`: The unique identifier of sslCertificate
  - `[SubcategoryTemplateId <String>]`: The unique identifier of subcategoryTemplate
  - `[SubdomainId <String>]`: The unique identifier of subdomain
  - `[SubjectRightsRequestId <String>]`: The unique identifier of subjectRightsRequest
  - `[TrainingId <String>]`: The unique identifier of training
  - `[TrainingLanguageDetailId <String>]`: The unique identifier of trainingLanguageDetail
  - `[UnifiedGroupSourceId <String>]`: The unique identifier of unifiedGroupSource
  - `[UserId <String>]`: The unique identifier of user
  - `[UserPrincipalName <String>]`: Alternate key of user
  - `[UserSourceId <String>]`: The unique identifier of userSource
  - `[VulnerabilityComponentId <String>]`: The unique identifier of vulnerabilityComponent
  - `[VulnerabilityId <String>]`: The unique identifier of vulnerability
  - `[WhoisHistoryRecordId <String>]`: The unique identifier of whoisHistoryRecord
  - `[WhoisRecordId <String>]`: The unique identifier of whoisRecord

SEARCH `<IMicrosoftGraphSecurityEdiscoverySearch>`: ediscoverySearch
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ContentQuery <String>]`:
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CreatedDateTime <DateTime?>]`:
  - `[Description <String>]`:
  - `[DisplayName <String>]`:
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[LastModifiedDateTime <DateTime?>]`:
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AddToReviewSetOperation <IMicrosoftGraphSecurityEdiscoveryAddToReviewSetOperation>]`: ediscoveryAddToReviewSetOperation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Action <String>]`: caseAction
    - `[CompletedDateTime <DateTime?>]`: The date and time the operation was completed.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: The date and time the operation was created.
    - `[PercentProgress <Int32?>]`: The progress of the operation.
    - `[ResultInfo <IMicrosoftGraphResultInfo>]`: resultInfo
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Code <Int32?>]`: The result code.
      - `[Message <String>]`: The message.
      - `[Subcode <Int32?>]`: The result subcode.
    - `[Status <String>]`: caseOperationStatus
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AdditionalDataOptions <String>]`: additionalDataOptions
    - `[CloudAttachmentVersion <String>]`: cloudAttachmentVersion
    - `[DocumentVersion <String>]`: documentVersion
    - `[ItemsToInclude <String>]`: itemsToInclude
    - `[ReviewSet <IMicrosoftGraphSecurityEdiscoveryReviewSet>]`: ediscoveryReviewSet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`:
      - `[Description <String>]`:
      - `[DisplayName <String>]`:
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Queries <IMicrosoftGraphSecurityEdiscoveryReviewSetQuery- `[]`>]`: Represents queries within the review set.
        - `[ContentQuery <String>]`:
        - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[CreatedDateTime <DateTime?>]`:
        - `[Description <String>]`:
        - `[DisplayName <String>]`:
        - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[LastModifiedDateTime <DateTime?>]`:
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Search <IMicrosoftGraphSecurityEdiscoverySearch>]`: ediscoverySearch
  - `[AdditionalSources <IMicrosoftGraphSecurityDataSource- `[]`>]`: Adds an additional source to the eDiscovery search.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: The date and time the dataSource was created.
    - `[DisplayName <String>]`: The display name of the dataSource and is the name of the SharePoint site.
    - `[HoldStatus <String>]`: dataSourceHoldStatus
  - `[CustodianSources <IMicrosoftGraphSecurityDataSource- `[]`>]`: Custodian sources that are included in the eDiscovery search.
  - `[DataSourceScopes <String>]`: dataSourceScopes
  - `[LastEstimateStatisticsOperation <IMicrosoftGraphSecurityEdiscoveryEstimateOperation>]`: ediscoveryEstimateOperation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Action <String>]`: caseAction
    - `[CompletedDateTime <DateTime?>]`: The date and time the operation was completed.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: The date and time the operation was created.
    - `[PercentProgress <Int32?>]`: The progress of the operation.
    - `[ResultInfo <IMicrosoftGraphResultInfo>]`: resultInfo
    - `[Status <String>]`: caseOperationStatus
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[IndexedItemCount <Int64?>]`: The estimated count of items for the search that matched the content query.
    - `[IndexedItemsSize <Int64?>]`: The estimated size of items for the search that matched the content query.
    - `[MailboxCount <Int32?>]`: The number of mailboxes that had search hits.
    - `[Search <IMicrosoftGraphSecurityEdiscoverySearch>]`: ediscoverySearch
    - `[SiteCount <Int32?>]`: The number of mailboxes that had search hits.
    - `[StatisticsOptions <String>]`: statisticsOptions
    - `[UnindexedItemCount <Int64?>]`: The estimated count of unindexed items for the collection.
    - `[UnindexedItemsSize <Int64?>]`: The estimated size of unindexed items for the collection.
  - `[NoncustodialSources <IMicrosoftGraphSecurityEdiscoveryNoncustodialDataSource- `[]`>]`: noncustodialDataSource sources that are included in the eDiscovery search
    - `[CreatedDateTime <DateTime?>]`: Created date and time of the dataSourceContainer entity.
    - `[DisplayName <String>]`: Display name of the dataSourceContainer entity.
    - `[HoldStatus <String>]`: dataSourceHoldStatus
    - `[LastModifiedDateTime <DateTime?>]`: Last modified date and time of the dataSourceContainer.
    - `[ReleasedDateTime <DateTime?>]`: Date and time that the dataSourceContainer was released from the case.
    - `[Status <String>]`: dataSourceContainerStatus
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DataSource <IMicrosoftGraphSecurityDataSource>]`: dataSource
    - `[LastIndexOperation <IMicrosoftGraphSecurityEdiscoveryIndexOperation>]`: ediscoveryIndexOperation
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Action <String>]`: caseAction
      - `[CompletedDateTime <DateTime?>]`: The date and time the operation was completed.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: The date and time the operation was created.
      - `[PercentProgress <Int32?>]`: The progress of the operation.
      - `[ResultInfo <IMicrosoftGraphResultInfo>]`: resultInfo
      - `[Status <String>]`: caseOperationStatus
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.security/add-mgsecuritycaseediscoverycasereviewsettoreviewset](https://learn.microsoft.com/powershell/module/microsoft.graph.security/add-mgsecuritycaseediscoverycasereviewsettoreviewset)

[https://learn.microsoft.com/graph/api/security-ediscoveryreviewset-addtoreviewset?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/security-ediscoveryreviewset-addtoreviewset?view=graph-rest-1.0)























