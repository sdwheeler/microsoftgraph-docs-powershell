---
external help file: Microsoft.Graph.Sites-help.xml
Module Name: Microsoft.Graph.Sites
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.sites/update-mgsitegetbypathtermstore
schema: 2.0.0
---

# Update-MgSiteGetByPathTermStore

## SYNOPSIS
Update the navigation property termStore in sites

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaSiteGetByPathTermStore](/powershell/module/Microsoft.Graph.Beta.Sites/Update-MgBetaSiteGetByPathTermStore?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgSiteGetByPathTermStore -Path <String> -SiteId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-DefaultLanguageTag <String>] [-Groups <IMicrosoftGraphTermStoreGroup[]>]
 [-Id <String>] [-LanguageTags <String[]>] [-Sets <IMicrosoftGraphTermStoreSet[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgSiteGetByPathTermStore -Path <String> -SiteId <String> -BodyParameter <IMicrosoftGraphTermStore>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgSiteGetByPathTermStore -InputObject <ISitesIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-DefaultLanguageTag <String>] [-Groups <IMicrosoftGraphTermStoreGroup[]>]
 [-Id <String>] [-LanguageTags <String[]>] [-Sets <IMicrosoftGraphTermStoreSet[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgSiteGetByPathTermStore -InputObject <ISitesIdentity> -BodyParameter <IMicrosoftGraphTermStore>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property termStore in sites

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

### -BodyParameter
store
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTermStore
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

### -DefaultLanguageTag
Default language of the term store.

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

### -Groups
Collection of all groups available in the term store.
To construct, see NOTES section for GROUPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTermStoreGroup[]
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ISitesIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LanguageTags
List of languages for the term store.

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

### -Path
Usage: path='{path}'

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

### -Sets
Collection of all sets available in the term store.
This relationship can only be used to load a specific term set.
To construct, see NOTES section for SETS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTermStoreSet[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, Update
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTermStore
### Microsoft.Graph.PowerShell.Models.ISitesIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTermStore
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphTermStore>`: store
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DefaultLanguageTag <String>]`: Default language of the term store.
  - `[Groups <IMicrosoftGraphTermStoreGroup- `[]`>]`: Collection of all groups available in the term store.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedDateTime <DateTime?>]`: Date and time of the group creation.
Read-only.
    - `[Description <String>]`: Description that gives details on the term usage.
    - `[DisplayName <String>]`: Name of the group.
    - `[ParentSiteId <String>]`: ID of the parent site of this group.
    - `[Scope <String>]`: termGroupScope
    - `[Sets <IMicrosoftGraphTermStoreSet- `[]`>]`: All sets under the group in a term - `[store]`.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Children <IMicrosoftGraphTermStoreTerm- `[]`>]`: Children terms of set in term - `[store]`.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[Children <IMicrosoftGraphTermStoreTerm- `[]`>]`: Children of current term.
        - `[CreatedDateTime <DateTime?>]`: Date and time of term creation.
Read-only.
        - `[Descriptions <IMicrosoftGraphTermStoreLocalizedDescription- `[]`>]`: Description about term that is dependent on the languageTag.
          - `[Description <String>]`: The description in the localized language.
          - `[LanguageTag <String>]`: The language tag for the label.
        - `[Labels <IMicrosoftGraphTermStoreLocalizedLabel- `[]`>]`: Label metadata for a term.
          - `[IsDefault <Boolean?>]`: Indicates whether the label is the default label.
          - `[LanguageTag <String>]`: The language tag for the label.
          - `[Name <String>]`: The name of the label.
        - `[LastModifiedDateTime <DateTime?>]`: Last date and time of term modification.
Read-only.
        - `[Properties <IMicrosoftGraphKeyValue- `[]`>]`: Collection of properties on the term.
          - `[Key <String>]`: Key for the key-value pair.
          - `[Value <String>]`: Value for the key-value pair.
        - `[Relations <IMicrosoftGraphTermStoreRelation- `[]`>]`: To indicate which terms are related to the current term as either pinned or reused.
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
          - `[FromTerm <IMicrosoftGraphTermStoreTerm>]`: term
          - `[Relationship <String>]`: relationType
          - `[Set <IMicrosoftGraphTermStoreSet>]`: set
          - `[ToTerm <IMicrosoftGraphTermStoreTerm>]`: term
        - `[Set <IMicrosoftGraphTermStoreSet>]`: set
      - `[CreatedDateTime <DateTime?>]`: Date and time of set creation.
Read-only.
      - `[Description <String>]`: Description that gives details on the term usage.
      - `[LocalizedNames <IMicrosoftGraphTermStoreLocalizedName- `[]`>]`: Name of the set for each languageTag.
        - `[LanguageTag <String>]`: The language tag for the label.
        - `[Name <String>]`: The name in the localized language.
      - `[ParentGroup <IMicrosoftGraphTermStoreGroup>]`: group
      - `[Properties <IMicrosoftGraphKeyValue- `[]`>]`: Custom properties for the set.
      - `[Relations <IMicrosoftGraphTermStoreRelation- `[]`>]`: Indicates which terms have been pinned or reused directly under the set.
      - `[Terms <IMicrosoftGraphTermStoreTerm- `[]`>]`: All the terms under the set.
  - `[LanguageTags <String- `[]`>]`: List of languages for the term store.
  - `[Sets <IMicrosoftGraphTermStoreSet- `[]`>]`: Collection of all sets available in the term store.
This relationship can only be used to load a specific term set.

GROUPS `<IMicrosoftGraphTermStoreGroup- `[]`>`: Collection of all groups available in the term store.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CreatedDateTime <DateTime?>]`: Date and time of the group creation.
Read-only.
  - `[Description <String>]`: Description that gives details on the term usage.
  - `[DisplayName <String>]`: Name of the group.
  - `[ParentSiteId <String>]`: ID of the parent site of this group.
  - `[Scope <String>]`: termGroupScope
  - `[Sets <IMicrosoftGraphTermStoreSet- `[]`>]`: All sets under the group in a term - `[store]`.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Children <IMicrosoftGraphTermStoreTerm- `[]`>]`: Children terms of set in term - `[store]`.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Children <IMicrosoftGraphTermStoreTerm- `[]`>]`: Children of current term.
      - `[CreatedDateTime <DateTime?>]`: Date and time of term creation.
Read-only.
      - `[Descriptions <IMicrosoftGraphTermStoreLocalizedDescription- `[]`>]`: Description about term that is dependent on the languageTag.
        - `[Description <String>]`: The description in the localized language.
        - `[LanguageTag <String>]`: The language tag for the label.
      - `[Labels <IMicrosoftGraphTermStoreLocalizedLabel- `[]`>]`: Label metadata for a term.
        - `[IsDefault <Boolean?>]`: Indicates whether the label is the default label.
        - `[LanguageTag <String>]`: The language tag for the label.
        - `[Name <String>]`: The name of the label.
      - `[LastModifiedDateTime <DateTime?>]`: Last date and time of term modification.
Read-only.
      - `[Properties <IMicrosoftGraphKeyValue- `[]`>]`: Collection of properties on the term.
        - `[Key <String>]`: Key for the key-value pair.
        - `[Value <String>]`: Value for the key-value pair.
      - `[Relations <IMicrosoftGraphTermStoreRelation- `[]`>]`: To indicate which terms are related to the current term as either pinned or reused.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[FromTerm <IMicrosoftGraphTermStoreTerm>]`: term
        - `[Relationship <String>]`: relationType
        - `[Set <IMicrosoftGraphTermStoreSet>]`: set
        - `[ToTerm <IMicrosoftGraphTermStoreTerm>]`: term
      - `[Set <IMicrosoftGraphTermStoreSet>]`: set
    - `[CreatedDateTime <DateTime?>]`: Date and time of set creation.
Read-only.
    - `[Description <String>]`: Description that gives details on the term usage.
    - `[LocalizedNames <IMicrosoftGraphTermStoreLocalizedName- `[]`>]`: Name of the set for each languageTag.
      - `[LanguageTag <String>]`: The language tag for the label.
      - `[Name <String>]`: The name in the localized language.
    - `[ParentGroup <IMicrosoftGraphTermStoreGroup>]`: group
    - `[Properties <IMicrosoftGraphKeyValue- `[]`>]`: Custom properties for the set.
    - `[Relations <IMicrosoftGraphTermStoreRelation- `[]`>]`: Indicates which terms have been pinned or reused directly under the set.
    - `[Terms <IMicrosoftGraphTermStoreTerm- `[]`>]`: All the terms under the set.

INPUTOBJECT `<ISitesIdentity>`: Identity Parameter
  - `[BaseItemId <String>]`: The unique identifier of baseItem
  - `[BaseSitePageId <String>]`: The unique identifier of baseSitePage
  - `[ColumnDefinitionId <String>]`: The unique identifier of columnDefinition
  - `[ColumnLinkId <String>]`: The unique identifier of columnLink
  - `[ContentTypeId <String>]`: The unique identifier of contentType
  - `[ContentTypeId1 <String>]`: The unique identifier of contentType
  - `[DocumentSetVersionId <String>]`: The unique identifier of documentSetVersion
  - `[DriveId <String>]`: The unique identifier of drive
  - `[EndDateTime <String>]`: Usage: endDateTime='{endDateTime}'
  - `[GroupId <String>]`: The unique identifier of group
  - `[GroupId1 <String>]`: The unique identifier of group
  - `[HorizontalSectionColumnId <String>]`: The unique identifier of horizontalSectionColumn
  - `[HorizontalSectionId <String>]`: The unique identifier of horizontalSection
  - `[IncludePersonalNotebooks <Boolean?>]`: Usage: includePersonalNotebooks={includePersonalNotebooks}
  - `[Interval <String>]`: Usage: interval='{interval}'
  - `[ItemActivityId <String>]`: The unique identifier of itemActivity
  - `[ItemActivityStatId <String>]`: The unique identifier of itemActivityStat
  - `[ListId <String>]`: The unique identifier of list
  - `[ListItemId <String>]`: The unique identifier of listItem
  - `[ListItemVersionId <String>]`: The unique identifier of listItemVersion
  - `[NotebookId <String>]`: The unique identifier of notebook
  - `[OnenoteOperationId <String>]`: The unique identifier of onenoteOperation
  - `[OnenotePageId <String>]`: The unique identifier of onenotePage
  - `[OnenoteResourceId <String>]`: The unique identifier of onenoteResource
  - `[OnenoteSectionId <String>]`: The unique identifier of onenoteSection
  - `[Path <String>]`: Usage: path='{path}'
  - `[PermissionId <String>]`: The unique identifier of permission
  - `[RelationId <String>]`: The unique identifier of relation
  - `[RichLongRunningOperationId <String>]`: The unique identifier of richLongRunningOperation
  - `[SectionGroupId <String>]`: The unique identifier of sectionGroup
  - `[SectionGroupId1 <String>]`: The unique identifier of sectionGroup
  - `[SetId <String>]`: The unique identifier of set
  - `[SetId1 <String>]`: The unique identifier of set
  - `[SiteId <String>]`: The unique identifier of site
  - `[SiteId1 <String>]`: The unique identifier of site
  - `[StartDateTime <String>]`: Usage: startDateTime='{startDateTime}'
  - `[StoreId <String>]`: The unique identifier of store
  - `[SubscriptionId <String>]`: The unique identifier of subscription
  - `[TermId <String>]`: The unique identifier of term
  - `[TermId1 <String>]`: The unique identifier of term
  - `[Token <String>]`: Usage: token='{token}'
  - `[UserId <String>]`: The unique identifier of user
  - `[WebPartId <String>]`: The unique identifier of webPart

SETS `<IMicrosoftGraphTermStoreSet- `[]`>`: Collection of all sets available in the term store.
This relationship can only be used to load a specific term set.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Children <IMicrosoftGraphTermStoreTerm- `[]`>]`: Children terms of set in term - `[store]`.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Children <IMicrosoftGraphTermStoreTerm- `[]`>]`: Children of current term.
    - `[CreatedDateTime <DateTime?>]`: Date and time of term creation.
Read-only.
    - `[Descriptions <IMicrosoftGraphTermStoreLocalizedDescription- `[]`>]`: Description about term that is dependent on the languageTag.
      - `[Description <String>]`: The description in the localized language.
      - `[LanguageTag <String>]`: The language tag for the label.
    - `[Labels <IMicrosoftGraphTermStoreLocalizedLabel- `[]`>]`: Label metadata for a term.
      - `[IsDefault <Boolean?>]`: Indicates whether the label is the default label.
      - `[LanguageTag <String>]`: The language tag for the label.
      - `[Name <String>]`: The name of the label.
    - `[LastModifiedDateTime <DateTime?>]`: Last date and time of term modification.
Read-only.
    - `[Properties <IMicrosoftGraphKeyValue- `[]`>]`: Collection of properties on the term.
      - `[Key <String>]`: Key for the key-value pair.
      - `[Value <String>]`: Value for the key-value pair.
    - `[Relations <IMicrosoftGraphTermStoreRelation- `[]`>]`: To indicate which terms are related to the current term as either pinned or reused.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[FromTerm <IMicrosoftGraphTermStoreTerm>]`: term
      - `[Relationship <String>]`: relationType
      - `[Set <IMicrosoftGraphTermStoreSet>]`: set
      - `[ToTerm <IMicrosoftGraphTermStoreTerm>]`: term
    - `[Set <IMicrosoftGraphTermStoreSet>]`: set
  - `[CreatedDateTime <DateTime?>]`: Date and time of set creation.
Read-only.
  - `[Description <String>]`: Description that gives details on the term usage.
  - `[LocalizedNames <IMicrosoftGraphTermStoreLocalizedName- `[]`>]`: Name of the set for each languageTag.
    - `[LanguageTag <String>]`: The language tag for the label.
    - `[Name <String>]`: The name in the localized language.
  - `[ParentGroup <IMicrosoftGraphTermStoreGroup>]`: group
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedDateTime <DateTime?>]`: Date and time of the group creation.
Read-only.
    - `[Description <String>]`: Description that gives details on the term usage.
    - `[DisplayName <String>]`: Name of the group.
    - `[ParentSiteId <String>]`: ID of the parent site of this group.
    - `[Scope <String>]`: termGroupScope
    - `[Sets <IMicrosoftGraphTermStoreSet- `[]`>]`: All sets under the group in a term - `[store]`.
  - `[Properties <IMicrosoftGraphKeyValue- `[]`>]`: Custom properties for the set.
  - `[Relations <IMicrosoftGraphTermStoreRelation- `[]`>]`: Indicates which terms have been pinned or reused directly under the set.
  - `[Terms <IMicrosoftGraphTermStoreTerm- `[]`>]`: All the terms under the set.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.sites/update-mgsitegetbypathtermstore](https://learn.microsoft.com/powershell/module/microsoft.graph.sites/update-mgsitegetbypathtermstore)
























