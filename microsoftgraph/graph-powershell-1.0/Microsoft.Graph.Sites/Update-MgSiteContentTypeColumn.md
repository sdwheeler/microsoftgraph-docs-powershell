---
external help file: Microsoft.Graph.Sites-help.xml
Module Name: Microsoft.Graph.Sites
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.sites/update-mgsitecontenttypecolumn
schema: 2.0.0
ms.subservice: sharepoint
---

# Update-MgSiteContentTypeColumn

## SYNOPSIS
Update a site, a list, or a content type column.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaSiteContentTypeColumn](/powershell/module/Microsoft.Graph.Beta.Sites/Update-MgBetaSiteContentTypeColumn?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgSiteContentTypeColumn -ColumnDefinitionId <String> -ContentTypeId <String> -SiteId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Boolean <Hashtable>]
 [-Calculated <IMicrosoftGraphCalculatedColumn>] [-Choice <IMicrosoftGraphChoiceColumn>]
 [-ColumnGroup <String>] [-ContentApprovalStatus <Hashtable>] [-Currency <IMicrosoftGraphCurrencyColumn>]
 [-DateTime <IMicrosoftGraphDateTimeColumn>] [-DefaultValue <IMicrosoftGraphDefaultColumnValue>]
 [-Description <String>] [-DisplayName <String>] [-EnforceUniqueValues] [-Geolocation <Hashtable>] [-Hidden]
 [-HyperlinkOrPicture <IMicrosoftGraphHyperlinkOrPictureColumn>] [-Id <String>] [-Indexed] [-IsDeletable]
 [-IsReorderable] [-IsSealed] [-Lookup <IMicrosoftGraphLookupColumn>] [-Name <String>]
 [-Number <IMicrosoftGraphNumberColumn>] [-PersonOrGroup <IMicrosoftGraphPersonOrGroupColumn>]
 [-PropagateChanges] [-ReadOnly] [-Required] [-SourceColumn <IMicrosoftGraphColumnDefinition>]
 [-SourceContentType <IMicrosoftGraphContentTypeInfo>] [-Term <IMicrosoftGraphTermColumn>]
 [-Text <IMicrosoftGraphTextColumn>] [-Thumbnail <Hashtable>] [-Type <String>]
 [-Validation <IMicrosoftGraphColumnValidation>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgSiteContentTypeColumn -ColumnDefinitionId <String> -ContentTypeId <String> -SiteId <String>
 -BodyParameter <IMicrosoftGraphColumnDefinition> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgSiteContentTypeColumn -InputObject <ISitesIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Boolean <Hashtable>] [-Calculated <IMicrosoftGraphCalculatedColumn>]
 [-Choice <IMicrosoftGraphChoiceColumn>] [-ColumnGroup <String>] [-ContentApprovalStatus <Hashtable>]
 [-Currency <IMicrosoftGraphCurrencyColumn>] [-DateTime <IMicrosoftGraphDateTimeColumn>]
 [-DefaultValue <IMicrosoftGraphDefaultColumnValue>] [-Description <String>] [-DisplayName <String>]
 [-EnforceUniqueValues] [-Geolocation <Hashtable>] [-Hidden]
 [-HyperlinkOrPicture <IMicrosoftGraphHyperlinkOrPictureColumn>] [-Id <String>] [-Indexed] [-IsDeletable]
 [-IsReorderable] [-IsSealed] [-Lookup <IMicrosoftGraphLookupColumn>] [-Name <String>]
 [-Number <IMicrosoftGraphNumberColumn>] [-PersonOrGroup <IMicrosoftGraphPersonOrGroupColumn>]
 [-PropagateChanges] [-ReadOnly] [-Required] [-SourceColumn <IMicrosoftGraphColumnDefinition>]
 [-SourceContentType <IMicrosoftGraphContentTypeInfo>] [-Term <IMicrosoftGraphTermColumn>]
 [-Text <IMicrosoftGraphTextColumn>] [-Thumbnail <Hashtable>] [-Type <String>]
 [-Validation <IMicrosoftGraphColumnValidation>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgSiteContentTypeColumn -InputObject <ISitesIdentity> -BodyParameter <IMicrosoftGraphColumnDefinition>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update a site, a list, or a content type column.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Sites.Manage.All, Sites.FullControl.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Sites.Manage.All, Sites.FullControl.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
	required = $true
	hidden = $false
	propagateChanges = $false
}

Update-MgSiteContentTypeColumn -SiteId $siteId -ContentTypeId $contentTypeId -ColumnDefinitionId $columnDefinitionId -BodyParameter $params

```
This example shows how to use the Update-MgSiteContentTypeColumn Cmdlet.


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
columnDefinition
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphColumnDefinition
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Boolean
booleanColumn

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

### -Calculated
calculatedColumn
To construct, see NOTES section for CALCULATED properties and create a hash table.

```yaml
Type: IMicrosoftGraphCalculatedColumn
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Choice
choiceColumn
To construct, see NOTES section for CHOICE properties and create a hash table.

```yaml
Type: IMicrosoftGraphChoiceColumn
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ColumnDefinitionId
The unique identifier of columnDefinition

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

### -ColumnGroup
For site columns, the name of the group this column belongs to.
Helps organize related columns.

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

### -ContentApprovalStatus
contentApprovalStatusColumn

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

### -ContentTypeId
The unique identifier of contentType

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

### -Currency
currencyColumn
To construct, see NOTES section for CURRENCY properties and create a hash table.

```yaml
Type: IMicrosoftGraphCurrencyColumn
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DateTime
dateTimeColumn
To construct, see NOTES section for DATETIME properties and create a hash table.

```yaml
Type: IMicrosoftGraphDateTimeColumn
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultValue
defaultColumnValue
To construct, see NOTES section for DEFAULTVALUE properties and create a hash table.

```yaml
Type: IMicrosoftGraphDefaultColumnValue
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
The user-facing description of the column.

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

### -DisplayName
The user-facing name of the column.

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

### -EnforceUniqueValues
If true, no two list items may have the same value for this column.

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

### -Geolocation
geolocationColumn

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

### -Hidden
Specifies whether the column is displayed in the user interface.

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

### -HyperlinkOrPicture
hyperlinkOrPictureColumn
To construct, see NOTES section for HYPERLINKORPICTURE properties and create a hash table.

```yaml
Type: IMicrosoftGraphHyperlinkOrPictureColumn
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### -Indexed
Specifies whether the column values can be used for sorting and searching.

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

### -IsDeletable
Indicates whether this column can be deleted.

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

### -IsReorderable
Indicates whether values in the column can be reordered.
Read-only.

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

### -IsSealed
Specifies whether the column can be changed.

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

### -Lookup
lookupColumn
To construct, see NOTES section for LOOKUP properties and create a hash table.

```yaml
Type: IMicrosoftGraphLookupColumn
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
The API-facing name of the column as it appears in the fields on a listItem.
For the user-facing name, see displayName.

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

### -Number
numberColumn
To construct, see NOTES section for NUMBER properties and create a hash table.

```yaml
Type: IMicrosoftGraphNumberColumn
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PersonOrGroup
personOrGroupColumn
To construct, see NOTES section for PERSONORGROUP properties and create a hash table.

```yaml
Type: IMicrosoftGraphPersonOrGroupColumn
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PropagateChanges
If 'true', changes to this column will be propagated to lists that implement the column.

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

### -ReadOnly
Specifies whether the column values can be modified.

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

### -Required
Specifies whether the column value isn't optional.

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
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourceColumn
columnDefinition
To construct, see NOTES section for SOURCECOLUMN properties and create a hash table.

```yaml
Type: IMicrosoftGraphColumnDefinition
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourceContentType
contentTypeInfo
To construct, see NOTES section for SOURCECONTENTTYPE properties and create a hash table.

```yaml
Type: IMicrosoftGraphContentTypeInfo
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Term
termColumn
To construct, see NOTES section for TERM properties and create a hash table.

```yaml
Type: IMicrosoftGraphTermColumn
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Text
textColumn
To construct, see NOTES section for TEXT properties and create a hash table.

```yaml
Type: IMicrosoftGraphTextColumn
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Thumbnail
thumbnailColumn

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

### -Type
columnTypes

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

### -Validation
columnValidation
To construct, see NOTES section for VALIDATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphColumnValidation
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphColumnDefinition
### Microsoft.Graph.PowerShell.Models.ISitesIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphColumnDefinition
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphColumnDefinition>`: columnDefinition
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Boolean <IMicrosoftGraphBooleanColumn>]`: booleanColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Calculated <IMicrosoftGraphCalculatedColumn>]`: calculatedColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Format <String>]`: For dateTime output types, the format of the value.
Possible values are: dateOnly or dateTime.
    - `[Formula <String>]`: The formula used to compute the value for this column.
    - `[OutputType <String>]`: The output type used to format values in this column.
Possible values are: boolean, currency, dateTime, number, or text.
  - `[Choice <IMicrosoftGraphChoiceColumn>]`: choiceColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowTextEntry <Boolean?>]`: If true, allows custom values that aren't in the configured choices.
    - `[Choices <String- `[]`>]`: The list of values available for this column.
    - `[DisplayAs <String>]`: How the choices are to be presented in the UX.
Must be one of checkBoxes, dropDownMenu, or radioButtons
  - `[ColumnGroup <String>]`: For site columns, the name of the group this column belongs to.
Helps organize related columns.
  - `[ContentApprovalStatus <IMicrosoftGraphContentApprovalStatusColumn>]`: contentApprovalStatusColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Currency <IMicrosoftGraphCurrencyColumn>]`: currencyColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Locale <String>]`: Specifies the locale from which to infer the currency symbol.
  - `[DateTime <IMicrosoftGraphDateTimeColumn>]`: dateTimeColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayAs <String>]`: How the value should be presented in the UX.
Must be one of default, friendly, or standard.
See below for more details.
If unspecified, treated as default.
    - `[Format <String>]`: Indicates whether the value should be presented as a date only or a date and time.
Must be one of dateOnly or dateTime
  - `[DefaultValue <IMicrosoftGraphDefaultColumnValue>]`: defaultColumnValue
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Formula <String>]`: The formula used to compute the default value for the column.
    - `[Value <String>]`: The direct value to use as the default value for the column.
  - `[Description <String>]`: The user-facing description of the column.
  - `[DisplayName <String>]`: The user-facing name of the column.
  - `[EnforceUniqueValues <Boolean?>]`: If true, no two list items may have the same value for this column.
  - `[Geolocation <IMicrosoftGraphGeolocationColumn>]`: geolocationColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Hidden <Boolean?>]`: Specifies whether the column is displayed in the user interface.
  - `[HyperlinkOrPicture <IMicrosoftGraphHyperlinkOrPictureColumn>]`: hyperlinkOrPictureColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsPicture <Boolean?>]`: Specifies whether the display format used for URL columns is an image or a hyperlink.
  - `[Indexed <Boolean?>]`: Specifies whether the column values can be used for sorting and searching.
  - `[IsDeletable <Boolean?>]`: Indicates whether this column can be deleted.
  - `[IsReorderable <Boolean?>]`: Indicates whether values in the column can be reordered.
Read-only.
  - `[IsSealed <Boolean?>]`: Specifies whether the column can be changed.
  - `[Lookup <IMicrosoftGraphLookupColumn>]`: lookupColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowMultipleValues <Boolean?>]`: Indicates whether multiple values can be selected from the source.
    - `[AllowUnlimitedLength <Boolean?>]`: Indicates whether values in the column should be able to exceed the standard limit of 255 characters.
    - `[ColumnName <String>]`: The name of the lookup source column.
    - `[ListId <String>]`: The unique identifier of the lookup source list.
    - `[PrimaryLookupColumnId <String>]`: If specified, this column is a secondary lookup, pulling an additional field from the list item looked up by the primary lookup.
Use the list item looked up by the primary as the source for the column named here.
  - `[Name <String>]`: The API-facing name of the column as it appears in the fields on a listItem.
For the user-facing name, see displayName.
  - `[Number <IMicrosoftGraphNumberColumn>]`: numberColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DecimalPlaces <String>]`: How many decimal places to display.
See below for information about the possible values.
    - `[DisplayAs <String>]`: How the value should be presented in the UX.
Must be one of number or percentage.
If unspecified, treated as number.
    - `[Maximum <Double?>]`: The maximum permitted value.
    - `[Minimum <Double?>]`: The minimum permitted value.
  - `[PersonOrGroup <IMicrosoftGraphPersonOrGroupColumn>]`: personOrGroupColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowMultipleSelection <Boolean?>]`: Indicates whether multiple values can be selected from the source.
    - `[ChooseFromType <String>]`: Whether to allow selection of people only, or people and groups.
Must be one of peopleAndGroups or peopleOnly.
    - `[DisplayAs <String>]`: How to display the information about the person or group chosen.
See below.
  - `[PropagateChanges <Boolean?>]`: If 'true', changes to this column will be propagated to lists that implement the column.
  - `[ReadOnly <Boolean?>]`: Specifies whether the column values can be modified.
  - `[Required <Boolean?>]`: Specifies whether the column value isn't optional.
  - `[SourceColumn <IMicrosoftGraphColumnDefinition>]`: columnDefinition
  - `[SourceContentType <IMicrosoftGraphContentTypeInfo>]`: contentTypeInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The ID of the content type.
    - `[Name <String>]`: The name of the content type.
  - `[Term <IMicrosoftGraphTermColumn>]`: termColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowMultipleValues <Boolean?>]`: Specifies whether the column allows more than one value.
    - `[ParentTerm <IMicrosoftGraphTermStoreTerm>]`: term
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
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
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
          - `[Children <IMicrosoftGraphTermStoreTerm- `[]`>]`: Children terms of set in term - `[store]`.
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
        - `[ToTerm <IMicrosoftGraphTermStoreTerm>]`: term
      - `[Set <IMicrosoftGraphTermStoreSet>]`: set
    - `[ShowFullyQualifiedName <Boolean?>]`: Specifies whether to display the entire term path or only the term label.
    - `[TermSet <IMicrosoftGraphTermStoreSet>]`: set
  - `[Text <IMicrosoftGraphTextColumn>]`: textColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowMultipleLines <Boolean?>]`: Whether to allow multiple lines of text.
    - `[AppendChangesToExistingText <Boolean?>]`: Whether updates to this column should replace existing text, or append to it.
    - `[LinesForEditing <Int32?>]`: The size of the text box.
    - `[MaxLength <Int32?>]`: The maximum number of characters for the value.
    - `[TextType <String>]`: The type of text being stored.
Must be one of plain or richText
  - `[Thumbnail <IMicrosoftGraphThumbnailColumn>]`: thumbnailColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Type <String>]`: columnTypes
  - `[Validation <IMicrosoftGraphColumnValidation>]`: columnValidation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DefaultLanguage <String>]`: Default BCP 47 language tag for the description.
    - `[Descriptions <IMicrosoftGraphDisplayNameLocalization- `[]`>]`: Localized messages that explain what is needed for this column's value to be considered valid.
User will be prompted with this message if validation fails.
      - `[DisplayName <String>]`: If present, the value of this field contains the displayName string that has been set for the language present in the languageTag field.
      - `[LanguageTag <String>]`: Provides the language culture-code and friendly name of the language that the displayName field has been provided in.
    - `[Formula <String>]`: The formula to validate column value.
For examples, see Examples of common formulas in lists.

CALCULATED `<IMicrosoftGraphCalculatedColumn>`: calculatedColumn
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Format <String>]`: For dateTime output types, the format of the value.
Possible values are: dateOnly or dateTime.
  - `[Formula <String>]`: The formula used to compute the value for this column.
  - `[OutputType <String>]`: The output type used to format values in this column.
Possible values are: boolean, currency, dateTime, number, or text.

CHOICE `<IMicrosoftGraphChoiceColumn>`: choiceColumn
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AllowTextEntry <Boolean?>]`: If true, allows custom values that aren't in the configured choices.
  - `[Choices <String- `[]`>]`: The list of values available for this column.
  - `[DisplayAs <String>]`: How the choices are to be presented in the UX.
Must be one of checkBoxes, dropDownMenu, or radioButtons

CURRENCY `<IMicrosoftGraphCurrencyColumn>`: currencyColumn
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Locale <String>]`: Specifies the locale from which to infer the currency symbol.

DATETIME `<IMicrosoftGraphDateTimeColumn>`: dateTimeColumn
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DisplayAs <String>]`: How the value should be presented in the UX.
Must be one of default, friendly, or standard.
See below for more details.
If unspecified, treated as default.
  - `[Format <String>]`: Indicates whether the value should be presented as a date only or a date and time.
Must be one of dateOnly or dateTime

DEFAULTVALUE `<IMicrosoftGraphDefaultColumnValue>`: defaultColumnValue
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Formula <String>]`: The formula used to compute the default value for the column.
  - `[Value <String>]`: The direct value to use as the default value for the column.

HYPERLINKORPICTURE `<IMicrosoftGraphHyperlinkOrPictureColumn>`: hyperlinkOrPictureColumn
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsPicture <Boolean?>]`: Specifies whether the display format used for URL columns is an image or a hyperlink.

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

LOOKUP `<IMicrosoftGraphLookupColumn>`: lookupColumn
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AllowMultipleValues <Boolean?>]`: Indicates whether multiple values can be selected from the source.
  - `[AllowUnlimitedLength <Boolean?>]`: Indicates whether values in the column should be able to exceed the standard limit of 255 characters.
  - `[ColumnName <String>]`: The name of the lookup source column.
  - `[ListId <String>]`: The unique identifier of the lookup source list.
  - `[PrimaryLookupColumnId <String>]`: If specified, this column is a secondary lookup, pulling an additional field from the list item looked up by the primary lookup.
Use the list item looked up by the primary as the source for the column named here.

NUMBER `<IMicrosoftGraphNumberColumn>`: numberColumn
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DecimalPlaces <String>]`: How many decimal places to display.
See below for information about the possible values.
  - `[DisplayAs <String>]`: How the value should be presented in the UX.
Must be one of number or percentage.
If unspecified, treated as number.
  - `[Maximum <Double?>]`: The maximum permitted value.
  - `[Minimum <Double?>]`: The minimum permitted value.

PERSONORGROUP `<IMicrosoftGraphPersonOrGroupColumn>`: personOrGroupColumn
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AllowMultipleSelection <Boolean?>]`: Indicates whether multiple values can be selected from the source.
  - `[ChooseFromType <String>]`: Whether to allow selection of people only, or people and groups.
Must be one of peopleAndGroups or peopleOnly.
  - `[DisplayAs <String>]`: How to display the information about the person or group chosen.
See below.

SOURCECOLUMN `<IMicrosoftGraphColumnDefinition>`: columnDefinition
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Boolean <IMicrosoftGraphBooleanColumn>]`: booleanColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Calculated <IMicrosoftGraphCalculatedColumn>]`: calculatedColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Format <String>]`: For dateTime output types, the format of the value.
Possible values are: dateOnly or dateTime.
    - `[Formula <String>]`: The formula used to compute the value for this column.
    - `[OutputType <String>]`: The output type used to format values in this column.
Possible values are: boolean, currency, dateTime, number, or text.
  - `[Choice <IMicrosoftGraphChoiceColumn>]`: choiceColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowTextEntry <Boolean?>]`: If true, allows custom values that aren't in the configured choices.
    - `[Choices <String- `[]`>]`: The list of values available for this column.
    - `[DisplayAs <String>]`: How the choices are to be presented in the UX.
Must be one of checkBoxes, dropDownMenu, or radioButtons
  - `[ColumnGroup <String>]`: For site columns, the name of the group this column belongs to.
Helps organize related columns.
  - `[ContentApprovalStatus <IMicrosoftGraphContentApprovalStatusColumn>]`: contentApprovalStatusColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Currency <IMicrosoftGraphCurrencyColumn>]`: currencyColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Locale <String>]`: Specifies the locale from which to infer the currency symbol.
  - `[DateTime <IMicrosoftGraphDateTimeColumn>]`: dateTimeColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayAs <String>]`: How the value should be presented in the UX.
Must be one of default, friendly, or standard.
See below for more details.
If unspecified, treated as default.
    - `[Format <String>]`: Indicates whether the value should be presented as a date only or a date and time.
Must be one of dateOnly or dateTime
  - `[DefaultValue <IMicrosoftGraphDefaultColumnValue>]`: defaultColumnValue
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Formula <String>]`: The formula used to compute the default value for the column.
    - `[Value <String>]`: The direct value to use as the default value for the column.
  - `[Description <String>]`: The user-facing description of the column.
  - `[DisplayName <String>]`: The user-facing name of the column.
  - `[EnforceUniqueValues <Boolean?>]`: If true, no two list items may have the same value for this column.
  - `[Geolocation <IMicrosoftGraphGeolocationColumn>]`: geolocationColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Hidden <Boolean?>]`: Specifies whether the column is displayed in the user interface.
  - `[HyperlinkOrPicture <IMicrosoftGraphHyperlinkOrPictureColumn>]`: hyperlinkOrPictureColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsPicture <Boolean?>]`: Specifies whether the display format used for URL columns is an image or a hyperlink.
  - `[Indexed <Boolean?>]`: Specifies whether the column values can be used for sorting and searching.
  - `[IsDeletable <Boolean?>]`: Indicates whether this column can be deleted.
  - `[IsReorderable <Boolean?>]`: Indicates whether values in the column can be reordered.
Read-only.
  - `[IsSealed <Boolean?>]`: Specifies whether the column can be changed.
  - `[Lookup <IMicrosoftGraphLookupColumn>]`: lookupColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowMultipleValues <Boolean?>]`: Indicates whether multiple values can be selected from the source.
    - `[AllowUnlimitedLength <Boolean?>]`: Indicates whether values in the column should be able to exceed the standard limit of 255 characters.
    - `[ColumnName <String>]`: The name of the lookup source column.
    - `[ListId <String>]`: The unique identifier of the lookup source list.
    - `[PrimaryLookupColumnId <String>]`: If specified, this column is a secondary lookup, pulling an additional field from the list item looked up by the primary lookup.
Use the list item looked up by the primary as the source for the column named here.
  - `[Name <String>]`: The API-facing name of the column as it appears in the fields on a listItem.
For the user-facing name, see displayName.
  - `[Number <IMicrosoftGraphNumberColumn>]`: numberColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DecimalPlaces <String>]`: How many decimal places to display.
See below for information about the possible values.
    - `[DisplayAs <String>]`: How the value should be presented in the UX.
Must be one of number or percentage.
If unspecified, treated as number.
    - `[Maximum <Double?>]`: The maximum permitted value.
    - `[Minimum <Double?>]`: The minimum permitted value.
  - `[PersonOrGroup <IMicrosoftGraphPersonOrGroupColumn>]`: personOrGroupColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowMultipleSelection <Boolean?>]`: Indicates whether multiple values can be selected from the source.
    - `[ChooseFromType <String>]`: Whether to allow selection of people only, or people and groups.
Must be one of peopleAndGroups or peopleOnly.
    - `[DisplayAs <String>]`: How to display the information about the person or group chosen.
See below.
  - `[PropagateChanges <Boolean?>]`: If 'true', changes to this column will be propagated to lists that implement the column.
  - `[ReadOnly <Boolean?>]`: Specifies whether the column values can be modified.
  - `[Required <Boolean?>]`: Specifies whether the column value isn't optional.
  - `[SourceColumn <IMicrosoftGraphColumnDefinition>]`: columnDefinition
  - `[SourceContentType <IMicrosoftGraphContentTypeInfo>]`: contentTypeInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The ID of the content type.
    - `[Name <String>]`: The name of the content type.
  - `[Term <IMicrosoftGraphTermColumn>]`: termColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowMultipleValues <Boolean?>]`: Specifies whether the column allows more than one value.
    - `[ParentTerm <IMicrosoftGraphTermStoreTerm>]`: term
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
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
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
          - `[Children <IMicrosoftGraphTermStoreTerm- `[]`>]`: Children terms of set in term - `[store]`.
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
        - `[ToTerm <IMicrosoftGraphTermStoreTerm>]`: term
      - `[Set <IMicrosoftGraphTermStoreSet>]`: set
    - `[ShowFullyQualifiedName <Boolean?>]`: Specifies whether to display the entire term path or only the term label.
    - `[TermSet <IMicrosoftGraphTermStoreSet>]`: set
  - `[Text <IMicrosoftGraphTextColumn>]`: textColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowMultipleLines <Boolean?>]`: Whether to allow multiple lines of text.
    - `[AppendChangesToExistingText <Boolean?>]`: Whether updates to this column should replace existing text, or append to it.
    - `[LinesForEditing <Int32?>]`: The size of the text box.
    - `[MaxLength <Int32?>]`: The maximum number of characters for the value.
    - `[TextType <String>]`: The type of text being stored.
Must be one of plain or richText
  - `[Thumbnail <IMicrosoftGraphThumbnailColumn>]`: thumbnailColumn
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Type <String>]`: columnTypes
  - `[Validation <IMicrosoftGraphColumnValidation>]`: columnValidation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DefaultLanguage <String>]`: Default BCP 47 language tag for the description.
    - `[Descriptions <IMicrosoftGraphDisplayNameLocalization- `[]`>]`: Localized messages that explain what is needed for this column's value to be considered valid.
User will be prompted with this message if validation fails.
      - `[DisplayName <String>]`: If present, the value of this field contains the displayName string that has been set for the language present in the languageTag field.
      - `[LanguageTag <String>]`: Provides the language culture-code and friendly name of the language that the displayName field has been provided in.
    - `[Formula <String>]`: The formula to validate column value.
For examples, see Examples of common formulas in lists.

SOURCECONTENTTYPE `<IMicrosoftGraphContentTypeInfo>`: contentTypeInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The ID of the content type.
  - `[Name <String>]`: The name of the content type.

TERM `<IMicrosoftGraphTermColumn>`: termColumn
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AllowMultipleValues <Boolean?>]`: Specifies whether the column allows more than one value.
  - `[ParentTerm <IMicrosoftGraphTermStoreTerm>]`: term
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
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
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[Children <IMicrosoftGraphTermStoreTerm- `[]`>]`: Children terms of set in term - `[store]`.
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
      - `[ToTerm <IMicrosoftGraphTermStoreTerm>]`: term
    - `[Set <IMicrosoftGraphTermStoreSet>]`: set
  - `[ShowFullyQualifiedName <Boolean?>]`: Specifies whether to display the entire term path or only the term label.
  - `[TermSet <IMicrosoftGraphTermStoreSet>]`: set

TEXT `<IMicrosoftGraphTextColumn>`: textColumn
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AllowMultipleLines <Boolean?>]`: Whether to allow multiple lines of text.
  - `[AppendChangesToExistingText <Boolean?>]`: Whether updates to this column should replace existing text, or append to it.
  - `[LinesForEditing <Int32?>]`: The size of the text box.
  - `[MaxLength <Int32?>]`: The maximum number of characters for the value.
  - `[TextType <String>]`: The type of text being stored.
Must be one of plain or richText

VALIDATION `<IMicrosoftGraphColumnValidation>`: columnValidation
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DefaultLanguage <String>]`: Default BCP 47 language tag for the description.
  - `[Descriptions <IMicrosoftGraphDisplayNameLocalization- `[]`>]`: Localized messages that explain what is needed for this column's value to be considered valid.
User will be prompted with this message if validation fails.
    - `[DisplayName <String>]`: If present, the value of this field contains the displayName string that has been set for the language present in the languageTag field.
    - `[LanguageTag <String>]`: Provides the language culture-code and friendly name of the language that the displayName field has been provided in.
  - `[Formula <String>]`: The formula to validate column value.
For examples, see Examples of common formulas in lists.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.sites/update-mgsitecontenttypecolumn](https://learn.microsoft.com/powershell/module/microsoft.graph.sites/update-mgsitecontenttypecolumn)

[https://learn.microsoft.com/graph/api/columndefinition-update?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/columndefinition-update?view=graph-rest-1.0)























