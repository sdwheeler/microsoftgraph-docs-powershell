---
external help file: Microsoft.Graph.Security-help.xml
Module Name: Microsoft.Graph.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.security/update-mgsecuritylabel
schema: 2.0.0
---

# Update-MgSecurityLabel

## SYNOPSIS
Update the navigation property labels in security

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaSecurityLabel](/powershell/module/Microsoft.Graph.Beta.Security/Update-MgBetaSecurityLabel?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgSecurityLabel [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Authorities <IMicrosoftGraphSecurityAuthorityTemplate[]>]
 [-Categories <IMicrosoftGraphSecurityCategoryTemplate[]>]
 [-Citations <IMicrosoftGraphSecurityCitationTemplate[]>]
 [-Departments <IMicrosoftGraphSecurityDepartmentTemplate[]>]
 [-FilePlanReferences <IMicrosoftGraphSecurityFilePlanReferenceTemplate[]>] [-Id <String>]
 [-RetentionLabels <IMicrosoftGraphSecurityRetentionLabel[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgSecurityLabel -BodyParameter <IMicrosoftGraphSecurityLabelsRoot> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property labels in security

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Authorities
Specifies the underlying authority that describes the type of content to be retained and its retention schedule.
To construct, see NOTES section for AUTHORITIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityAuthorityTemplate[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
labelsRoot
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityLabelsRoot
Parameter Sets: Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Categories
Specifies a group of similar types of content in a particular department.
To construct, see NOTES section for CATEGORIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityCategoryTemplate[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Citations
The specific rule or regulation created by a jurisdiction used to determine whether certain labels and content should be retained or deleted.
To construct, see NOTES section for CITATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityCitationTemplate[]
Parameter Sets: UpdateExpanded
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

### -Departments
Specifies the department or business unit of an organization to which a label belongs.
To construct, see NOTES section for DEPARTMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityDepartmentTemplate[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FilePlanReferences
Specifies a unique alpha-numeric identifier for an organization's retention schedule.
To construct, see NOTES section for FILEPLANREFERENCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityFilePlanReferenceTemplate[]
Parameter Sets: UpdateExpanded
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
Parameter Sets: UpdateExpanded
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

### -RetentionLabels
Represents how customers can manage their data, whether and for how long to retain or delete it.
To construct, see NOTES section for RETENTIONLABELS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityRetentionLabel[]
Parameter Sets: UpdateExpanded
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphSecurityLabelsRoot
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphSecurityLabelsRoot
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

AUTHORITIES `<IMicrosoftGraphSecurityAuthorityTemplate- `[]`>`: Specifies the underlying authority that describes the type of content to be retained and its retention schedule.
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
  - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
  - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

BODYPARAMETER `<IMicrosoftGraphSecurityLabelsRoot>`: labelsRoot
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Authorities <IMicrosoftGraphSecurityAuthorityTemplate- `[]`>]`: Specifies the underlying authority that describes the type of content to be retained and its retention schedule.
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
    - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
    - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Categories <IMicrosoftGraphSecurityCategoryTemplate- `[]`>]`: Specifies a group of similar types of content in a particular department.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
    - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Subcategories <IMicrosoftGraphSecuritySubcategoryTemplate- `[]`>]`: Represents all subcategories under a particular category.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
      - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Citations <IMicrosoftGraphSecurityCitationTemplate- `[]`>]`: The specific rule or regulation created by a jurisdiction used to determine whether certain labels and content should be retained or deleted.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
    - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CitationJurisdiction <String>]`: Represents the jurisdiction or agency that published the citation.
    - `[CitationUrl <String>]`: Represents the URL to the published citation.
  - `[Departments <IMicrosoftGraphSecurityDepartmentTemplate- `[]`>]`: Specifies the department or business unit of an organization to which a label belongs.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
    - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[FilePlanReferences <IMicrosoftGraphSecurityFilePlanReferenceTemplate- `[]`>]`: Specifies a unique alpha-numeric identifier for an organization's retention schedule.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
    - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[RetentionLabels <IMicrosoftGraphSecurityRetentionLabel- `[]`>]`: Represents how customers can manage their data, whether and for how long to retain or delete it.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ActionAfterRetentionPeriod <String>]`: actionAfterRetentionPeriod
    - `[BehaviorDuringRetentionPeriod <String>]`: behaviorDuringRetentionPeriod
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the retentionLabel is created.
    - `[DefaultRecordBehavior <String>]`: defaultRecordBehavior
    - `[DescriptionForAdmins <String>]`: Provides label information for the admin.
Optional.
    - `[DescriptionForUsers <String>]`: Provides the label information for the user.
Optional.
    - `[Descriptors <IMicrosoftGraphSecurityFilePlanDescriptor>]`: filePlanDescriptor
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Authority <IMicrosoftGraphSecurityFilePlanAuthority>]`: filePlanAuthority
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
      - `[AuthorityTemplate <IMicrosoftGraphSecurityAuthorityTemplate>]`: authorityTemplate
      - `[Category <IMicrosoftGraphSecurityFilePlanAppliedCategory>]`: filePlanAppliedCategory
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
        - `[Subcategory <IMicrosoftGraphSecurityFilePlanSubcategory>]`: filePlanSubcategory
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
      - `[CategoryTemplate <IMicrosoftGraphSecurityCategoryTemplate>]`: categoryTemplate
      - `[Citation <IMicrosoftGraphSecurityFilePlanCitation>]`: filePlanCitation
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
        - `[CitationJurisdiction <String>]`: Represents the jurisdiction or agency that published the filePlanCitation.
        - `[CitationUrl <String>]`: Represents the URL to the published filePlanCitation.
      - `[CitationTemplate <IMicrosoftGraphSecurityCitationTemplate>]`: citationTemplate
      - `[Department <IMicrosoftGraphSecurityFilePlanDepartment>]`: filePlanDepartment
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
      - `[DepartmentTemplate <IMicrosoftGraphSecurityDepartmentTemplate>]`: departmentTemplate
      - `[FilePlanReference <IMicrosoftGraphSecurityFilePlanReference>]`: filePlanReference
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
      - `[FilePlanReferenceTemplate <IMicrosoftGraphSecurityFilePlanReferenceTemplate>]`: filePlanReferenceTemplate
    - `[DisplayName <String>]`: Unique string that defines a label name.
    - `[DispositionReviewStages <IMicrosoftGraphSecurityDispositionReviewStage- `[]`>]`: When action at the end of retention is chosen as 'dispositionReview', dispositionReviewStages specifies a sequential set of stages with at least one reviewer in each stage.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Name <String>]`: Name representing each stage within a collection.
      - `[ReviewersEmailAddresses <String- `[]`>]`: A collection of reviewers at each stage.
      - `[StageNumber <String>]`: The unique sequence number for each stage of the disposition review.
    - `[IsInUse <Boolean?>]`: Specifies whether the label is currently being used.
    - `[LabelToBeApplied <String>]`: Specifies the replacement label to be applied automatically after the retention period of the current label ends.
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedDateTime <DateTime?>]`: The latest date time when the retentionLabel was modified.
    - `[RetentionDuration <IMicrosoftGraphSecurityRetentionDuration>]`: retentionDuration
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[RetentionEventType <IMicrosoftGraphSecurityRetentionEventType>]`: retentionEventType
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: The date time when the retentionEventType was created.
      - `[Description <String>]`: Optional information about the event type.
      - `[DisplayName <String>]`: Name of the event type.
      - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[LastModifiedDateTime <DateTime?>]`: The latest date time when the retentionEventType was modified.
    - `[RetentionTrigger <String>]`: retentionTrigger

CATEGORIES `<IMicrosoftGraphSecurityCategoryTemplate- `[]`>`: Specifies a group of similar types of content in a particular department.
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
  - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
  - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Subcategories <IMicrosoftGraphSecuritySubcategoryTemplate- `[]`>]`: Represents all subcategories under a particular category.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
    - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.

CITATIONS `<IMicrosoftGraphSecurityCitationTemplate- `[]`>`: The specific rule or regulation created by a jurisdiction used to determine whether certain labels and content should be retained or deleted.
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
  - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
  - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CitationJurisdiction <String>]`: Represents the jurisdiction or agency that published the citation.
  - `[CitationUrl <String>]`: Represents the URL to the published citation.

DEPARTMENTS `<IMicrosoftGraphSecurityDepartmentTemplate- `[]`>`: Specifies the department or business unit of an organization to which a label belongs.
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
  - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
  - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

FILEPLANREFERENCES `<IMicrosoftGraphSecurityFilePlanReferenceTemplate- `[]`>`: Specifies a unique alpha-numeric identifier for an organization's retention schedule.
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
  - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
  - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

RETENTIONLABELS `<IMicrosoftGraphSecurityRetentionLabel- `[]`>`: Represents how customers can manage their data, whether and for how long to retain or delete it.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActionAfterRetentionPeriod <String>]`: actionAfterRetentionPeriod
  - `[BehaviorDuringRetentionPeriod <String>]`: behaviorDuringRetentionPeriod
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
  - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the retentionLabel is created.
  - `[DefaultRecordBehavior <String>]`: defaultRecordBehavior
  - `[DescriptionForAdmins <String>]`: Provides label information for the admin.
Optional.
  - `[DescriptionForUsers <String>]`: Provides the label information for the user.
Optional.
  - `[Descriptors <IMicrosoftGraphSecurityFilePlanDescriptor>]`: filePlanDescriptor
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Authority <IMicrosoftGraphSecurityFilePlanAuthority>]`: filePlanAuthority
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
    - `[AuthorityTemplate <IMicrosoftGraphSecurityAuthorityTemplate>]`: authorityTemplate
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
      - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Category <IMicrosoftGraphSecurityFilePlanAppliedCategory>]`: filePlanAppliedCategory
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
      - `[Subcategory <IMicrosoftGraphSecurityFilePlanSubcategory>]`: filePlanSubcategory
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
    - `[CategoryTemplate <IMicrosoftGraphSecurityCategoryTemplate>]`: categoryTemplate
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
      - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Subcategories <IMicrosoftGraphSecuritySubcategoryTemplate- `[]`>]`: Represents all subcategories under a particular category.
        - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
        - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Citation <IMicrosoftGraphSecurityFilePlanCitation>]`: filePlanCitation
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
      - `[CitationJurisdiction <String>]`: Represents the jurisdiction or agency that published the filePlanCitation.
      - `[CitationUrl <String>]`: Represents the URL to the published filePlanCitation.
    - `[CitationTemplate <IMicrosoftGraphSecurityCitationTemplate>]`: citationTemplate
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
      - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CitationJurisdiction <String>]`: Represents the jurisdiction or agency that published the citation.
      - `[CitationUrl <String>]`: Represents the URL to the published citation.
    - `[Department <IMicrosoftGraphSecurityFilePlanDepartment>]`: filePlanDepartment
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
    - `[DepartmentTemplate <IMicrosoftGraphSecurityDepartmentTemplate>]`: departmentTemplate
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
      - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[FilePlanReference <IMicrosoftGraphSecurityFilePlanReference>]`: filePlanReference
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: Unique string that defines the name for the file plan descriptor associated with a particular retention label.
    - `[FilePlanReferenceTemplate <IMicrosoftGraphSecurityFilePlanReferenceTemplate>]`: filePlanReferenceTemplate
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
      - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: Unique string that defines a label name.
  - `[DispositionReviewStages <IMicrosoftGraphSecurityDispositionReviewStage- `[]`>]`: When action at the end of retention is chosen as 'dispositionReview', dispositionReviewStages specifies a sequential set of stages with at least one reviewer in each stage.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Name <String>]`: Name representing each stage within a collection.
    - `[ReviewersEmailAddresses <String- `[]`>]`: A collection of reviewers at each stage.
    - `[StageNumber <String>]`: The unique sequence number for each stage of the disposition review.
  - `[IsInUse <Boolean?>]`: Specifies whether the label is currently being used.
  - `[LabelToBeApplied <String>]`: Specifies the replacement label to be applied automatically after the retention period of the current label ends.
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[LastModifiedDateTime <DateTime?>]`: The latest date time when the retentionLabel was modified.
  - `[RetentionDuration <IMicrosoftGraphSecurityRetentionDuration>]`: retentionDuration
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[RetentionEventType <IMicrosoftGraphSecurityRetentionEventType>]`: retentionEventType
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: The date time when the retentionEventType was created.
    - `[Description <String>]`: Optional information about the event type.
    - `[DisplayName <String>]`: Name of the event type.
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedDateTime <DateTime?>]`: The latest date time when the retentionEventType was modified.
  - `[RetentionTrigger <String>]`: retentionTrigger

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.security/update-mgsecuritylabel](https://learn.microsoft.com/powershell/module/microsoft.graph.security/update-mgsecuritylabel)
























