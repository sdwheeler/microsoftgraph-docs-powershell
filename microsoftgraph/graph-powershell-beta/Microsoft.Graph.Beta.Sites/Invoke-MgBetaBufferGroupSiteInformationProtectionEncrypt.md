---
external help file: Microsoft.Graph.Beta.Sites-help.xml
Module Name: Microsoft.Graph.Beta.Sites
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.sites/invoke-mgbetabuffergroupsiteinformationprotectionencrypt
schema: 2.0.0
---

# Invoke-MgBetaBufferGroupSiteInformationProtectionEncrypt

## SYNOPSIS
Invoke action encryptBuffer

## SYNTAX

### BufferExpanded (Default)
```
Invoke-MgBetaBufferGroupSiteInformationProtectionEncrypt -GroupId <String> -SiteId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-BufferInputFile <String>]
 [-LabelId <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Buffer
```
Invoke-MgBetaBufferGroupSiteInformationProtectionEncrypt -GroupId <String> -SiteId <String>
 -Body <IPaths1G9H29GGroupsGroupIdSitesSiteIdInformationprotectionMicrosoftGraphEncryptbufferPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### BufferViaIdentityExpanded
```
Invoke-MgBetaBufferGroupSiteInformationProtectionEncrypt -InputObject <ISitesIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-BufferInputFile <String>]
 [-LabelId <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### BufferViaIdentity
```
Invoke-MgBetaBufferGroupSiteInformationProtectionEncrypt -InputObject <ISitesIdentity>
 [-ResponseHeadersVariable <String>]
 -BodyParameter <IPaths1G9H29GGroupsGroupIdSitesSiteIdInformationprotectionMicrosoftGraphEncryptbufferPostRequestbodyContentApplicationJsonSchema>
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action encryptBuffer

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: BufferExpanded, BufferViaIdentityExpanded
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
Type: IPaths1G9H29GGroupsGroupIdSitesSiteIdInformationprotectionMicrosoftGraphEncryptbufferPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Buffer
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BodyParameter

To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths1G9H29GGroupsGroupIdSitesSiteIdInformationprotectionMicrosoftGraphEncryptbufferPostRequestbodyContentApplicationJsonSchema
Parameter Sets: BufferViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BufferInputFile
Input File for Buffer (.)

```yaml
Type: String
Parameter Sets: BufferExpanded, BufferViaIdentityExpanded
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

### -GroupId
The unique identifier of group

```yaml
Type: String
Parameter Sets: BufferExpanded, Buffer
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
Type: ISitesIdentity
Parameter Sets: BufferViaIdentityExpanded, BufferViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LabelId


```yaml
Type: String
Parameter Sets: BufferExpanded, BufferViaIdentityExpanded
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

### -SiteId
The unique identifier of site

```yaml
Type: String
Parameter Sets: BufferExpanded, Buffer
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

### Microsoft.Graph.Beta.PowerShell.Models.IPaths1G9H29GGroupsGroupIdSitesSiteIdInformationprotectionMicrosoftGraphEncryptbufferPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.Beta.PowerShell.Models.ISitesIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphBufferEncryptionResult
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODY `<IPaths1G9H29GGroupsGroupIdSitesSiteIdInformationprotectionMicrosoftGraphEncryptbufferPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Buffer <Byte- `[]`>]`: 
  - `[LabelId <String>]`: 

BODYPARAMETER `<IPaths1G9H29GGroupsGroupIdSitesSiteIdInformationprotectionMicrosoftGraphEncryptbufferPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Buffer <Byte- `[]`>]`: 
  - `[LabelId <String>]`: 

INPUTOBJECT `<ISitesIdentity>`: Identity Parameter
  - `[BaseItemId <String>]`: The unique identifier of baseItem
  - `[BaseSitePageId <String>]`: The unique identifier of baseSitePage
  - `[BitlockerRecoveryKeyId <String>]`: The unique identifier of bitlockerRecoveryKey
  - `[ColumnDefinitionId <String>]`: The unique identifier of columnDefinition
  - `[ColumnLinkId <String>]`: The unique identifier of columnLink
  - `[ContentModelId <String>]`: The unique identifier of contentModel
  - `[ContentTypeId <String>]`: The unique identifier of contentType
  - `[ContentTypeId1 <String>]`: The unique identifier of contentType
  - `[DataLossPreventionPolicyId <String>]`: The unique identifier of dataLossPreventionPolicy
  - `[DocumentProcessingJobId <String>]`: The unique identifier of documentProcessingJob
  - `[DocumentSetVersionId <String>]`: The unique identifier of documentSetVersion
  - `[DriveId <String>]`: The unique identifier of drive
  - `[EndDateTime <String>]`: Usage: endDateTime='{endDateTime}'
  - `[GroupId <String>]`: The unique identifier of group
  - `[GroupId1 <String>]`: The unique identifier of group
  - `[HorizontalSectionColumnId <String>]`: The unique identifier of horizontalSectionColumn
  - `[HorizontalSectionId <String>]`: The unique identifier of horizontalSection
  - `[IncludePersonalNotebooks <Boolean?>]`: Usage: includePersonalNotebooks={includePersonalNotebooks}
  - `[InformationProtectionLabelId <String>]`: The unique identifier of informationProtectionLabel
  - `[Interval <String>]`: Usage: interval='{interval}'
  - `[ItemActivityId <String>]`: The unique identifier of itemActivity
  - `[ItemActivityOldId <String>]`: The unique identifier of itemActivityOLD
  - `[ItemActivityStatId <String>]`: The unique identifier of itemActivityStat
  - `[ListId <String>]`: The unique identifier of list
  - `[ListItemId <String>]`: The unique identifier of listItem
  - `[ListItemVersionId <String>]`: The unique identifier of listItemVersion
  - `[ModelName <String>]`: Usage: modelName='{modelName}'
  - `[NotebookId <String>]`: The unique identifier of notebook
  - `[OnenoteOperationId <String>]`: The unique identifier of onenoteOperation
  - `[OnenotePageId <String>]`: The unique identifier of onenotePage
  - `[OnenoteResourceId <String>]`: The unique identifier of onenoteResource
  - `[OnenoteSectionId <String>]`: The unique identifier of onenoteSection
  - `[PageTemplateId <String>]`: The unique identifier of pageTemplate
  - `[Path <String>]`: Usage: path='{path}'
  - `[PermissionId <String>]`: The unique identifier of permission
  - `[RecycleBinItemId <String>]`: The unique identifier of recycleBinItem
  - `[RelationId <String>]`: The unique identifier of relation
  - `[RichLongRunningOperationId <String>]`: The unique identifier of richLongRunningOperation
  - `[SectionGroupId <String>]`: The unique identifier of sectionGroup
  - `[SectionGroupId1 <String>]`: The unique identifier of sectionGroup
  - `[SensitivityLabelId <String>]`: The unique identifier of sensitivityLabel
  - `[SensitivityLabelId1 <String>]`: The unique identifier of sensitivityLabel
  - `[SetId <String>]`: The unique identifier of set
  - `[SetId1 <String>]`: The unique identifier of set
  - `[SiteId <String>]`: The unique identifier of site
  - `[SiteId1 <String>]`: The unique identifier of site
  - `[StartDateTime <String>]`: Usage: startDateTime='{startDateTime}'
  - `[SubscriptionId <String>]`: The unique identifier of subscription
  - `[TermId <String>]`: The unique identifier of term
  - `[TermId1 <String>]`: The unique identifier of term
  - `[ThreatAssessmentRequestId <String>]`: The unique identifier of threatAssessmentRequest
  - `[ThreatAssessmentResultId <String>]`: The unique identifier of threatAssessmentResult
  - `[Token <String>]`: Usage: token='{token}'
  - `[UserId <String>]`: The unique identifier of user
  - `[WebPartId <String>]`: The unique identifier of webPart

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.sites/invoke-mgbetabuffergroupsiteinformationprotectionencrypt](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.sites/invoke-mgbetabuffergroupsiteinformationprotectionencrypt)
























