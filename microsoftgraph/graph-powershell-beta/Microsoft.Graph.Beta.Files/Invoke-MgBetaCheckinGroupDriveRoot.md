---
external help file: Microsoft.Graph.Beta.Files-help.xml
Module Name: Microsoft.Graph.Beta.Files
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.files/invoke-mgbetacheckingroupdriveroot
schema: 2.0.0
ms.subservice: sharepoint
---

# Invoke-MgBetaCheckinGroupDriveRoot

## SYNOPSIS
Check in a checked out driveItem resource, which makes the version of the document available to others.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Invoke-MgCheckinGroupDriveRoot](/powershell/module/Microsoft.Graph.Files/Invoke-MgCheckinGroupDriveRoot?view=graph-powershell-1.0)

## SYNTAX

### CheckinExpanded (Default)
```
Invoke-MgBetaCheckinGroupDriveRoot -DriveId <String> -GroupId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CheckInAs <String>] [-Comment <String>] [-Headers <IDictionary>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Checkin
```
Invoke-MgBetaCheckinGroupDriveRoot -DriveId <String> -GroupId <String>
 -Body <IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CheckinViaIdentityExpanded
```
Invoke-MgBetaCheckinGroupDriveRoot -InputObject <IFilesIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CheckInAs <String>] [-Comment <String>] [-Headers <IDictionary>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CheckinViaIdentity
```
Invoke-MgBetaCheckinGroupDriveRoot -InputObject <IFilesIdentity> [-ResponseHeadersVariable <String>]
 -BodyParameter <IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema>
 [-Headers <IDictionary>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Check in a checked out driveItem resource, which makes the version of the document available to others.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CheckinExpanded, CheckinViaIdentityExpanded
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
Type: IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Checkin
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
Type: IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema
Parameter Sets: CheckinViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CheckInAs


```yaml
Type: String
Parameter Sets: CheckinExpanded, CheckinViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Comment


```yaml
Type: String
Parameter Sets: CheckinExpanded, CheckinViaIdentityExpanded
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

### -DriveId
The unique identifier of drive

```yaml
Type: String
Parameter Sets: CheckinExpanded, Checkin
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupId
The unique identifier of group

```yaml
Type: String
Parameter Sets: CheckinExpanded, Checkin
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
Parameter Sets: CheckinViaIdentityExpanded, CheckinViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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
### Microsoft.Graph.Beta.PowerShell.Models.IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODY `<IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CheckInAs <String>]`: 
  - `[Comment <String>]`: 

BODYPARAMETER `<IPathsD0Tb1DGroupsGroupIdDrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CheckInAs <String>]`: 
  - `[Comment <String>]`: 

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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.files/invoke-mgbetacheckingroupdriveroot](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.files/invoke-mgbetacheckingroupdriveroot)

[https://learn.microsoft.com/graph/api/driveitem-checkin?view=graph-rest-beta](https://learn.microsoft.com/graph/api/driveitem-checkin?view=graph-rest-beta)
























