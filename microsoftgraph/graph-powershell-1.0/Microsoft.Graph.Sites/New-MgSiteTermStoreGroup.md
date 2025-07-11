---
external help file: Microsoft.Graph.Sites-help.xml
Module Name: Microsoft.Graph.Sites
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.sites/new-mgsitetermstoregroup
schema: 2.0.0
ms.subservice: sharepoint
---

# New-MgSiteTermStoreGroup

## SYNOPSIS
Create a new group object in a term store.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaSiteTermStoreGroup](/powershell/module/Microsoft.Graph.Beta.Sites/New-MgBetaSiteTermStoreGroup?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgSiteTermStoreGroup -SiteId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>] [-Description <String>]
 [-DisplayName <String>] [-Id <String>] [-ParentSiteId <String>] [-Scope <String>]
 [-Sets <IMicrosoftGraphTermStoreSet[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateExpanded1
```
New-MgSiteTermStoreGroup -SiteId <String> -StoreId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>] [-Description <String>]
 [-DisplayName <String>] [-Id <String>] [-ParentSiteId <String>] [-Scope <String>]
 [-Sets <IMicrosoftGraphTermStoreSet[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create1
```
New-MgSiteTermStoreGroup -SiteId <String> -StoreId <String> -BodyParameter <IMicrosoftGraphTermStoreGroup>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgSiteTermStoreGroup -SiteId <String> -BodyParameter <IMicrosoftGraphTermStoreGroup>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded1
```
New-MgSiteTermStoreGroup -InputObject <ISitesIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>] [-Description <String>]
 [-DisplayName <String>] [-Id <String>] [-ParentSiteId <String>] [-Scope <String>]
 [-Sets <IMicrosoftGraphTermStoreSet[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgSiteTermStoreGroup -InputObject <ISitesIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>] [-Description <String>]
 [-DisplayName <String>] [-Id <String>] [-ParentSiteId <String>] [-Scope <String>]
 [-Sets <IMicrosoftGraphTermStoreSet[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity1
```
New-MgSiteTermStoreGroup -InputObject <ISitesIdentity> -BodyParameter <IMicrosoftGraphTermStoreGroup>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgSiteTermStoreGroup -InputObject <ISitesIdentity> -BodyParameter <IMicrosoftGraphTermStoreGroup>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new group object in a term store.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
	displayName = "myGroup"
}

New-MgSiteTermStoreGroup -SiteId $siteId -BodyParameter $params

```
This example shows how to use the New-MgSiteTermStoreGroup Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
group
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTermStoreGroup
Parameter Sets: Create1, Create, CreateViaIdentity1, CreateViaIdentity
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

### -CreatedDateTime
Date and time of the group creation.
Read-only.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
Description that gives details on the term usage.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Name of the group.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
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
Parameter Sets: CreateViaIdentityExpanded1, CreateViaIdentityExpanded, CreateViaIdentity1, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ParentSiteId
ID of the parent site of this group.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
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

### -Scope
termGroupScope

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sets
All sets under the group in a term \[store\].
To construct, see NOTES section for SETS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTermStoreSet[]
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateExpanded1, Create1, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StoreId
The unique identifier of store

```yaml
Type: String
Parameter Sets: CreateExpanded1, Create1
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTermStoreGroup
### Microsoft.Graph.PowerShell.Models.ISitesIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTermStoreGroup
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphTermStoreGroup>`: group
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

SETS `<IMicrosoftGraphTermStoreSet- `[]`>`: All sets under the group in a term - `[store]`.
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

[https://learn.microsoft.com/powershell/module/microsoft.graph.sites/new-mgsitetermstoregroup](https://learn.microsoft.com/powershell/module/microsoft.graph.sites/new-mgsitetermstoregroup)

[https://learn.microsoft.com/graph/api/termstore-group-post?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/termstore-group-post?view=graph-rest-1.0)























