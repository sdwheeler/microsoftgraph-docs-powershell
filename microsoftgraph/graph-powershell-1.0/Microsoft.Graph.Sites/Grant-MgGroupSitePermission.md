---
external help file: Microsoft.Graph.Sites-help.xml
Module Name: Microsoft.Graph.Sites
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.sites/grant-mggroupsitepermission
schema: 2.0.0
ms.subservice: sharepoint
---

# Grant-MgGroupSitePermission

## SYNOPSIS
Grant users access to a link represented by a permission.

> [!NOTE]
> To view the beta release of this cmdlet, view [Grant-MgBetaGroupSitePermission](/powershell/module/Microsoft.Graph.Beta.Sites/Grant-MgBetaGroupSitePermission?view=graph-powershell-beta)

## SYNTAX

### GrantExpanded (Default)
```
Grant-MgGroupSitePermission -GroupId <String> -PermissionId <String> -SiteId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Recipients <IMicrosoftGraphDriveRecipient[]>] [-Roles <String[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Grant
```
Grant-MgGroupSitePermission -GroupId <String> -PermissionId <String> -SiteId <String>
 -BodyParameter <IPaths1Bir9OcGroupsGroupIdSitesSiteIdPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### GrantViaIdentityExpanded
```
Grant-MgGroupSitePermission -InputObject <ISitesIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Recipients <IMicrosoftGraphDriveRecipient[]>] [-Roles <String[]>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GrantViaIdentity
```
Grant-MgGroupSitePermission -InputObject <ISitesIdentity>
 -BodyParameter <IPaths1Bir9OcGroupsGroupIdSitesSiteIdPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Grant users access to a link represented by a permission.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: GrantExpanded, GrantViaIdentityExpanded
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
Type: IPaths1Bir9OcGroupsGroupIdSitesSiteIdPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Grant, GrantViaIdentity
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

### -GroupId
The unique identifier of group

```yaml
Type: String
Parameter Sets: GrantExpanded, Grant
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
Parameter Sets: GrantViaIdentityExpanded, GrantViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PermissionId
The unique identifier of permission

```yaml
Type: String
Parameter Sets: GrantExpanded, Grant
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Recipients

To construct, see NOTES section for RECIPIENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDriveRecipient[]
Parameter Sets: GrantExpanded, GrantViaIdentityExpanded
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

### -Roles


```yaml
Type: String[]
Parameter Sets: GrantExpanded, GrantViaIdentityExpanded
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
Parameter Sets: GrantExpanded, Grant
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

### Microsoft.Graph.PowerShell.Models.IPaths1Bir9OcGroupsGroupIdSitesSiteIdPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.PowerShell.Models.ISitesIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPermission
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths1Bir9OcGroupsGroupIdSitesSiteIdPermissionsPermissionIdMicrosoftGraphGrantPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Recipients <IMicrosoftGraphDriveRecipient- `[]`>]`:
    - `[Alias <String>]`: The alias of the domain object, for cases where an email address is unavailable (e.g.
security groups).
    - `[Email <String>]`: The email address for the recipient, if the recipient has an associated email address.
    - `[ObjectId <String>]`: The unique identifier for the recipient in the directory.
  - `[Roles <String- `[]`>]`:

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

RECIPIENTS `<IMicrosoftGraphDriveRecipient- `[]`>`: .
  - `[Alias <String>]`: The alias of the domain object, for cases where an email address is unavailable (e.g.
security groups).
  - `[Email <String>]`: The email address for the recipient, if the recipient has an associated email address.
  - `[ObjectId <String>]`: The unique identifier for the recipient in the directory.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.sites/grant-mggroupsitepermission](https://learn.microsoft.com/powershell/module/microsoft.graph.sites/grant-mggroupsitepermission)

[https://learn.microsoft.com/graph/api/permission-grant?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/permission-grant?view=graph-rest-1.0)
























