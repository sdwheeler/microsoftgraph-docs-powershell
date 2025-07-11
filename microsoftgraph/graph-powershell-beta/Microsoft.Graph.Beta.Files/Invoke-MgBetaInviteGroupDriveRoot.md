---
external help file: Microsoft.Graph.Beta.Files-help.xml
Module Name: Microsoft.Graph.Beta.Files
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.files/invoke-mgbetainvitegroupdriveroot
schema: 2.0.0
ms.subservice: sharepoint
---

# Invoke-MgBetaInviteGroupDriveRoot

## SYNOPSIS
Sends a sharing invitation for a driveItem.A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Invoke-MgInviteGroupDriveRoot](/powershell/module/Microsoft.Graph.Files/Invoke-MgInviteGroupDriveRoot?view=graph-powershell-1.0)

## SYNTAX

### InviteExpanded (Default)
```
Invoke-MgBetaInviteGroupDriveRoot -DriveId <String> -GroupId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ExpirationDateTime <String>] [-Message <String>] [-Password <String>]
 [-Recipients <IMicrosoftGraphDriveRecipient[]>] [-RequireSignIn] [-RetainInheritedPermissions]
 [-Roles <String[]>] [-SendInvitation] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Invite
```
Invoke-MgBetaInviteGroupDriveRoot -DriveId <String> -GroupId <String>
 -BodyParameter <IPaths18Lmc20GroupsGroupIdDrivesDriveIdRootMicrosoftGraphInvitePostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### InviteViaIdentityExpanded
```
Invoke-MgBetaInviteGroupDriveRoot -InputObject <IFilesIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ExpirationDateTime <String>] [-Message <String>] [-Password <String>]
 [-Recipients <IMicrosoftGraphDriveRecipient[]>] [-RequireSignIn] [-RetainInheritedPermissions]
 [-Roles <String[]>] [-SendInvitation] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### InviteViaIdentity
```
Invoke-MgBetaInviteGroupDriveRoot -InputObject <IFilesIdentity>
 -BodyParameter <IPaths18Lmc20GroupsGroupIdDrivesDriveIdRootMicrosoftGraphInvitePostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Sends a sharing invitation for a driveItem.A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: InviteExpanded, InviteViaIdentityExpanded
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
Type: IPaths18Lmc20GroupsGroupIdDrivesDriveIdRootMicrosoftGraphInvitePostRequestbodyContentApplicationJsonSchema
Parameter Sets: Invite, InviteViaIdentity
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

### -DriveId
The unique identifier of drive

```yaml
Type: String
Parameter Sets: InviteExpanded, Invite
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpirationDateTime


```yaml
Type: String
Parameter Sets: InviteExpanded, InviteViaIdentityExpanded
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
Parameter Sets: InviteExpanded, Invite
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
Type: IFilesIdentity
Parameter Sets: InviteViaIdentityExpanded, InviteViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Message


```yaml
Type: String
Parameter Sets: InviteExpanded, InviteViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Password


```yaml
Type: String
Parameter Sets: InviteExpanded, InviteViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Recipients

To construct, see NOTES section for RECIPIENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDriveRecipient[]
Parameter Sets: InviteExpanded, InviteViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RequireSignIn


```yaml
Type: SwitchParameter
Parameter Sets: InviteExpanded, InviteViaIdentityExpanded
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

### -RetainInheritedPermissions


```yaml
Type: SwitchParameter
Parameter Sets: InviteExpanded, InviteViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Roles


```yaml
Type: String[]
Parameter Sets: InviteExpanded, InviteViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SendInvitation


```yaml
Type: SwitchParameter
Parameter Sets: InviteExpanded, InviteViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
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

### Microsoft.Graph.Beta.PowerShell.Models.IFilesIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IPaths18Lmc20GroupsGroupIdDrivesDriveIdRootMicrosoftGraphInvitePostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPermission
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths18Lmc20GroupsGroupIdDrivesDriveIdRootMicrosoftGraphInvitePostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ExpirationDateTime <String>]`: 
  - `[Message <String>]`: 
  - `[Password <String>]`: 
  - `[Recipients <IMicrosoftGraphDriveRecipient- `[]`>]`: 
    - `[Alias <String>]`: The alias of the domain object, for cases where an email address is unavailable (e.g.
security groups).
    - `[Email <String>]`: The email address for the recipient, if the recipient has an associated email address.
    - `[ObjectId <String>]`: The unique identifier for the recipient in the directory.
  - `[RequireSignIn <Boolean?>]`: 
  - `[RetainInheritedPermissions <Boolean?>]`: 
  - `[Roles <String- `[]`>]`: 
  - `[SendInvitation <Boolean?>]`: 

INPUTOBJECT `<IFilesIdentity>`: Identity Parameter
  - `[ColumnDefinitionId <String>]`: The unique identifier of columnDefinition
  - `[ColumnLinkId <String>]`: The unique identifier of columnLink
  - `[ContentTypeId <String>]`: The unique identifier of contentType
  - `[ContentTypeId1 <String>]`: The unique identifier of contentType
  - `[DocumentSetVersionId <String>]`: The unique identifier of documentSetVersion
  - `[DriveId <String>]`: The unique identifier of drive
  - `[DriveItemId <String>]`: The unique identifier of driveItem
  - `[DriveItemId1 <String>]`: The unique identifier of driveItem
  - `[DriveItemVersionId <String>]`: The unique identifier of driveItemVersion
  - `[EndDateTime <String>]`: Usage: endDateTime='{endDateTime}'
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[GroupId <String>]`: The unique identifier of group
  - `[Interval <String>]`: Usage: interval='{interval}'
  - `[ItemActivityStatId <String>]`: The unique identifier of itemActivityStat
  - `[ListItemId <String>]`: The unique identifier of listItem
  - `[ListItemVersionId <String>]`: The unique identifier of listItemVersion
  - `[PermissionId <String>]`: The unique identifier of permission
  - `[Q <String>]`: Usage: q='{q}'
  - `[RichLongRunningOperationId <String>]`: The unique identifier of richLongRunningOperation
  - `[SharedDriveItemId <String>]`: The unique identifier of sharedDriveItem
  - `[StartDateTime <String>]`: Usage: startDateTime='{startDateTime}'
  - `[SubscriptionId <String>]`: The unique identifier of subscription
  - `[ThumbnailSetId <String>]`: The unique identifier of thumbnailSet
  - `[Token <String>]`: Usage: token='{token}'
  - `[UserId <String>]`: The unique identifier of user

RECIPIENTS `<IMicrosoftGraphDriveRecipient- `[]`>`: .
  - `[Alias <String>]`: The alias of the domain object, for cases where an email address is unavailable (e.g.
security groups).
  - `[Email <String>]`: The email address for the recipient, if the recipient has an associated email address.
  - `[ObjectId <String>]`: The unique identifier for the recipient in the directory.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.files/invoke-mgbetainvitegroupdriveroot](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.files/invoke-mgbetainvitegroupdriveroot)

[https://learn.microsoft.com/graph/api/driveitem-invite?view=graph-rest-beta](https://learn.microsoft.com/graph/api/driveitem-invite?view=graph-rest-beta)
























