---
external help file: Microsoft.Graph.Beta.Sites-help.xml
Module Name: Microsoft.Graph.Beta.Sites
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.sites/new-mgbetagroupsiteonenotesectionpage
schema: 2.0.0
---

# New-MgBetaGroupSiteOnenoteSectionPage

## SYNOPSIS
Create new navigation property to pages for groups

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgGroupSiteOnenoteSectionPage](/powershell/module/Microsoft.Graph.Sites/New-MgGroupSiteOnenoteSectionPage?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaGroupSiteOnenoteSectionPage -GroupId <String> -OnenoteSectionId <String> -SiteId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-ContentInputFile <String>]
 [-ContentUrl <String>] [-CreatedByAppId <String>] [-CreatedDateTime <DateTime>] [-Id <String>]
 [-LastModifiedDateTime <DateTime>] [-Level <Int32>] [-Links <IMicrosoftGraphPageLinks>] [-Order <Int32>]
 [-ParentNotebook <IMicrosoftGraphNotebook>] [-ParentSection <IMicrosoftGraphOnenoteSection>] [-Self <String>]
 [-Title <String>] [-UserTags <String[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaGroupSiteOnenoteSectionPage -GroupId <String> -OnenoteSectionId <String> -SiteId <String>
 -BodyParameter <IMicrosoftGraphOnenotePage> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaGroupSiteOnenoteSectionPage -InputObject <ISitesIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ContentInputFile <String>] [-ContentUrl <String>]
 [-CreatedByAppId <String>] [-CreatedDateTime <DateTime>] [-Id <String>] [-LastModifiedDateTime <DateTime>]
 [-Level <Int32>] [-Links <IMicrosoftGraphPageLinks>] [-Order <Int32>]
 [-ParentNotebook <IMicrosoftGraphNotebook>] [-ParentSection <IMicrosoftGraphOnenoteSection>] [-Self <String>]
 [-Title <String>] [-UserTags <String[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaGroupSiteOnenoteSectionPage -InputObject <ISitesIdentity> -BodyParameter <IMicrosoftGraphOnenotePage>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to pages for groups

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
onenotePage
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphOnenotePage
Parameter Sets: Create, CreateViaIdentity
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

### -ContentInputFile
Input File for Content (The page's HTML content.)

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContentUrl
The URL for the page's HTML content.
Read-only.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedByAppId
The unique identifier of the application that created the page.
Read-only.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime


```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

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
Parameter Sets: CreateExpanded, Create
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Type: ISitesIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LastModifiedDateTime
The date and time when the page was last modified.
The timestamp represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Level
The indentation level of the page.
Read-only.

```yaml
Type: Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Links
pageLinks
To construct, see NOTES section for LINKS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPageLinks
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OnenoteSectionId
The unique identifier of onenoteSection

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Order
The order of the page within its parent section.
Read-only.

```yaml
Type: Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -ParentNotebook
notebook
To construct, see NOTES section for PARENTNOTEBOOK properties and create a hash table.

```yaml
Type: IMicrosoftGraphNotebook
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ParentSection
onenoteSection
To construct, see NOTES section for PARENTSECTION properties and create a hash table.

```yaml
Type: IMicrosoftGraphOnenoteSection
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### -Self


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

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
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Title
The title of the page.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserTags


```yaml
Type: String[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphOnenotePage
### Microsoft.Graph.Beta.PowerShell.Models.ISitesIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphOnenotePage
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphOnenotePage>`: onenotePage
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CreatedDateTime <DateTime?>]`: 
  - `[Self <String>]`: 
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Content <Byte- `[]`>]`: The page's HTML content.
  - `[ContentUrl <String>]`: The URL for the page's HTML content. 
Read-only.
  - `[CreatedByAppId <String>]`: The unique identifier of the application that created the page.
Read-only.
  - `[LastModifiedDateTime <DateTime?>]`: The date and time when the page was last modified.
The timestamp represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
  - `[Level <Int32?>]`: The indentation level of the page.
Read-only.
  - `[Links <IMicrosoftGraphPageLinks>]`: pageLinks
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[OneNoteClientUrl <IMicrosoftGraphExternalLink>]`: externalLink
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Href <String>]`: The URL of the link.
    - `[OneNoteWebUrl <IMicrosoftGraphExternalLink>]`: externalLink
  - `[Order <Int32?>]`: The order of the page within its parent section.
Read-only.
  - `[ParentNotebook <IMicrosoftGraphNotebook>]`: notebook
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
        - `[Id <String>]`: The identifier of the identity.
This property is read-only.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[DisplayName <String>]`: 
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedDateTime <DateTime?>]`: 
    - `[CreatedDateTime <DateTime?>]`: 
    - `[Self <String>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[IsDefault <Boolean?>]`: Indicates whether this is the user's default notebook.
Read-only.
    - `[IsShared <Boolean?>]`: Indicates whether the notebook is shared.
If true, the contents of the notebook can be seen by people other than the owner.
Read-only.
    - `[Links <IMicrosoftGraphNotebookLinks>]`: notebookLinks
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[OneNoteClientUrl <IMicrosoftGraphExternalLink>]`: externalLink
      - `[OneNoteWebUrl <IMicrosoftGraphExternalLink>]`: externalLink
    - `[SectionGroups <IMicrosoftGraphSectionGroup- `[]`>]`: The section groups in the notebook.
Read-only.
Nullable.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[DisplayName <String>]`: 
      - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[LastModifiedDateTime <DateTime?>]`: 
      - `[CreatedDateTime <DateTime?>]`: 
      - `[Self <String>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ParentNotebook <IMicrosoftGraphNotebook>]`: notebook
      - `[ParentSectionGroup <IMicrosoftGraphSectionGroup>]`: sectionGroup
      - `[SectionGroups <IMicrosoftGraphSectionGroup- `[]`>]`: The section groups in the section.
Read-only.
Nullable.
      - `[SectionGroupsUrl <String>]`: The URL for the sectionGroups navigation property, which returns all the section groups in the section group.
Read-only.
      - `[Sections <IMicrosoftGraphOnenoteSection- `[]`>]`: The sections in the section group.
Read-only.
Nullable.
        - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[DisplayName <String>]`: 
        - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[LastModifiedDateTime <DateTime?>]`: 
        - `[CreatedDateTime <DateTime?>]`: 
        - `[Self <String>]`: 
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[IsDefault <Boolean?>]`: Indicates whether this is the user's default section.
Read-only.
        - `[Links <IMicrosoftGraphSectionLinks>]`: sectionLinks
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[OneNoteClientUrl <IMicrosoftGraphExternalLink>]`: externalLink
          - `[OneNoteWebUrl <IMicrosoftGraphExternalLink>]`: externalLink
        - `[Pages <IMicrosoftGraphOnenotePage- `[]`>]`: The collection of pages in the section. 
Read-only.
Nullable.
        - `[PagesUrl <String>]`: The pages endpoint where you can get details for all the pages in the section.
Read-only.
        - `[ParentNotebook <IMicrosoftGraphNotebook>]`: notebook
        - `[ParentSectionGroup <IMicrosoftGraphSectionGroup>]`: sectionGroup
      - `[SectionsUrl <String>]`: The URL for the sections navigation property, which returns all the sections in the section group.
Read-only.
    - `[SectionGroupsUrl <String>]`: The URL for the sectionGroups navigation property, which returns all the section groups in the notebook.
Read-only.
    - `[Sections <IMicrosoftGraphOnenoteSection- `[]`>]`: The sections in the notebook.
Read-only.
Nullable.
    - `[SectionsUrl <String>]`: The URL for the sections navigation property, which returns all the sections in the notebook.
Read-only.
    - `[UserRole <String>]`: onenoteUserRole
  - `[ParentSection <IMicrosoftGraphOnenoteSection>]`: onenoteSection
  - `[Title <String>]`: The title of the page.
  - `[UserTags <String- `[]`>]`: 

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

LINKS `<IMicrosoftGraphPageLinks>`: pageLinks
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[OneNoteClientUrl <IMicrosoftGraphExternalLink>]`: externalLink
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Href <String>]`: The URL of the link.
  - `[OneNoteWebUrl <IMicrosoftGraphExternalLink>]`: externalLink

PARENTNOTEBOOK `<IMicrosoftGraphNotebook>`: notebook
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[DisplayName <String>]`: 
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[LastModifiedDateTime <DateTime?>]`: 
  - `[CreatedDateTime <DateTime?>]`: 
  - `[Self <String>]`: 
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[IsDefault <Boolean?>]`: Indicates whether this is the user's default notebook.
Read-only.
  - `[IsShared <Boolean?>]`: Indicates whether the notebook is shared.
If true, the contents of the notebook can be seen by people other than the owner.
Read-only.
  - `[Links <IMicrosoftGraphNotebookLinks>]`: notebookLinks
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[OneNoteClientUrl <IMicrosoftGraphExternalLink>]`: externalLink
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Href <String>]`: The URL of the link.
    - `[OneNoteWebUrl <IMicrosoftGraphExternalLink>]`: externalLink
  - `[SectionGroups <IMicrosoftGraphSectionGroup- `[]`>]`: The section groups in the notebook.
Read-only.
Nullable.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[DisplayName <String>]`: 
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedDateTime <DateTime?>]`: 
    - `[CreatedDateTime <DateTime?>]`: 
    - `[Self <String>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ParentNotebook <IMicrosoftGraphNotebook>]`: notebook
    - `[ParentSectionGroup <IMicrosoftGraphSectionGroup>]`: sectionGroup
    - `[SectionGroups <IMicrosoftGraphSectionGroup- `[]`>]`: The section groups in the section.
Read-only.
Nullable.
    - `[SectionGroupsUrl <String>]`: The URL for the sectionGroups navigation property, which returns all the section groups in the section group.
Read-only.
    - `[Sections <IMicrosoftGraphOnenoteSection- `[]`>]`: The sections in the section group.
Read-only.
Nullable.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[DisplayName <String>]`: 
      - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[LastModifiedDateTime <DateTime?>]`: 
      - `[CreatedDateTime <DateTime?>]`: 
      - `[Self <String>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[IsDefault <Boolean?>]`: Indicates whether this is the user's default section.
Read-only.
      - `[Links <IMicrosoftGraphSectionLinks>]`: sectionLinks
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[OneNoteClientUrl <IMicrosoftGraphExternalLink>]`: externalLink
        - `[OneNoteWebUrl <IMicrosoftGraphExternalLink>]`: externalLink
      - `[Pages <IMicrosoftGraphOnenotePage- `[]`>]`: The collection of pages in the section. 
Read-only.
Nullable.
        - `[CreatedDateTime <DateTime?>]`: 
        - `[Self <String>]`: 
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[Content <Byte- `[]`>]`: The page's HTML content.
        - `[ContentUrl <String>]`: The URL for the page's HTML content. 
Read-only.
        - `[CreatedByAppId <String>]`: The unique identifier of the application that created the page.
Read-only.
        - `[LastModifiedDateTime <DateTime?>]`: The date and time when the page was last modified.
The timestamp represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
        - `[Level <Int32?>]`: The indentation level of the page.
Read-only.
        - `[Links <IMicrosoftGraphPageLinks>]`: pageLinks
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[OneNoteClientUrl <IMicrosoftGraphExternalLink>]`: externalLink
          - `[OneNoteWebUrl <IMicrosoftGraphExternalLink>]`: externalLink
        - `[Order <Int32?>]`: The order of the page within its parent section.
Read-only.
        - `[ParentNotebook <IMicrosoftGraphNotebook>]`: notebook
        - `[ParentSection <IMicrosoftGraphOnenoteSection>]`: onenoteSection
        - `[Title <String>]`: The title of the page.
        - `[UserTags <String- `[]`>]`: 
      - `[PagesUrl <String>]`: The pages endpoint where you can get details for all the pages in the section.
Read-only.
      - `[ParentNotebook <IMicrosoftGraphNotebook>]`: notebook
      - `[ParentSectionGroup <IMicrosoftGraphSectionGroup>]`: sectionGroup
    - `[SectionsUrl <String>]`: The URL for the sections navigation property, which returns all the sections in the section group.
Read-only.
  - `[SectionGroupsUrl <String>]`: The URL for the sectionGroups navigation property, which returns all the section groups in the notebook.
Read-only.
  - `[Sections <IMicrosoftGraphOnenoteSection- `[]`>]`: The sections in the notebook.
Read-only.
Nullable.
  - `[SectionsUrl <String>]`: The URL for the sections navigation property, which returns all the sections in the notebook.
Read-only.
  - `[UserRole <String>]`: onenoteUserRole

PARENTSECTION `<IMicrosoftGraphOnenoteSection>`: onenoteSection
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[DisplayName <String>]`: 
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[LastModifiedDateTime <DateTime?>]`: 
  - `[CreatedDateTime <DateTime?>]`: 
  - `[Self <String>]`: 
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[IsDefault <Boolean?>]`: Indicates whether this is the user's default section.
Read-only.
  - `[Links <IMicrosoftGraphSectionLinks>]`: sectionLinks
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[OneNoteClientUrl <IMicrosoftGraphExternalLink>]`: externalLink
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Href <String>]`: The URL of the link.
    - `[OneNoteWebUrl <IMicrosoftGraphExternalLink>]`: externalLink
  - `[Pages <IMicrosoftGraphOnenotePage- `[]`>]`: The collection of pages in the section. 
Read-only.
Nullable.
    - `[CreatedDateTime <DateTime?>]`: 
    - `[Self <String>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Content <Byte- `[]`>]`: The page's HTML content.
    - `[ContentUrl <String>]`: The URL for the page's HTML content. 
Read-only.
    - `[CreatedByAppId <String>]`: The unique identifier of the application that created the page.
Read-only.
    - `[LastModifiedDateTime <DateTime?>]`: The date and time when the page was last modified.
The timestamp represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    - `[Level <Int32?>]`: The indentation level of the page.
Read-only.
    - `[Links <IMicrosoftGraphPageLinks>]`: pageLinks
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[OneNoteClientUrl <IMicrosoftGraphExternalLink>]`: externalLink
      - `[OneNoteWebUrl <IMicrosoftGraphExternalLink>]`: externalLink
    - `[Order <Int32?>]`: The order of the page within its parent section.
Read-only.
    - `[ParentNotebook <IMicrosoftGraphNotebook>]`: notebook
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[DisplayName <String>]`: 
      - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[LastModifiedDateTime <DateTime?>]`: 
      - `[CreatedDateTime <DateTime?>]`: 
      - `[Self <String>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[IsDefault <Boolean?>]`: Indicates whether this is the user's default notebook.
Read-only.
      - `[IsShared <Boolean?>]`: Indicates whether the notebook is shared.
If true, the contents of the notebook can be seen by people other than the owner.
Read-only.
      - `[Links <IMicrosoftGraphNotebookLinks>]`: notebookLinks
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[OneNoteClientUrl <IMicrosoftGraphExternalLink>]`: externalLink
        - `[OneNoteWebUrl <IMicrosoftGraphExternalLink>]`: externalLink
      - `[SectionGroups <IMicrosoftGraphSectionGroup- `[]`>]`: The section groups in the notebook.
Read-only.
Nullable.
        - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[DisplayName <String>]`: 
        - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[LastModifiedDateTime <DateTime?>]`: 
        - `[CreatedDateTime <DateTime?>]`: 
        - `[Self <String>]`: 
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[ParentNotebook <IMicrosoftGraphNotebook>]`: notebook
        - `[ParentSectionGroup <IMicrosoftGraphSectionGroup>]`: sectionGroup
        - `[SectionGroups <IMicrosoftGraphSectionGroup- `[]`>]`: The section groups in the section.
Read-only.
Nullable.
        - `[SectionGroupsUrl <String>]`: The URL for the sectionGroups navigation property, which returns all the section groups in the section group.
Read-only.
        - `[Sections <IMicrosoftGraphOnenoteSection- `[]`>]`: The sections in the section group.
Read-only.
Nullable.
        - `[SectionsUrl <String>]`: The URL for the sections navigation property, which returns all the sections in the section group.
Read-only.
      - `[SectionGroupsUrl <String>]`: The URL for the sectionGroups navigation property, which returns all the section groups in the notebook.
Read-only.
      - `[Sections <IMicrosoftGraphOnenoteSection- `[]`>]`: The sections in the notebook.
Read-only.
Nullable.
      - `[SectionsUrl <String>]`: The URL for the sections navigation property, which returns all the sections in the notebook.
Read-only.
      - `[UserRole <String>]`: onenoteUserRole
    - `[ParentSection <IMicrosoftGraphOnenoteSection>]`: onenoteSection
    - `[Title <String>]`: The title of the page.
    - `[UserTags <String- `[]`>]`: 
  - `[PagesUrl <String>]`: The pages endpoint where you can get details for all the pages in the section.
Read-only.
  - `[ParentNotebook <IMicrosoftGraphNotebook>]`: notebook
  - `[ParentSectionGroup <IMicrosoftGraphSectionGroup>]`: sectionGroup

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.sites/new-mgbetagroupsiteonenotesectionpage](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.sites/new-mgbetagroupsiteonenotesectionpage)
























