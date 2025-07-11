---
external help file: Microsoft.Graph.Beta.Files-help.xml
Module Name: Microsoft.Graph.Beta.Files
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.files/new-mgbetagroupdriveitemuploadsession
schema: 2.0.0
---

# New-MgBetaGroupDriveItemUploadSession

## SYNOPSIS
Invoke action createUploadSession

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgGroupDriveItemUploadSession](/powershell/module/Microsoft.Graph.Files/New-MgGroupDriveItemUploadSession?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaGroupDriveItemUploadSession -DriveId <String> -DriveItemId <String> -GroupId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Item <IMicrosoftGraphDriveItemUploadableProperties>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaGroupDriveItemUploadSession -DriveId <String> -DriveItemId <String> -GroupId <String>
 -BodyParameter <IPathsPpp20NGroupsGroupIdDrivesDriveIdItemsDriveitemIdMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaGroupDriveItemUploadSession -InputObject <IFilesIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Item <IMicrosoftGraphDriveItemUploadableProperties>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaGroupDriveItemUploadSession -InputObject <IFilesIdentity>
 -BodyParameter <IPathsPpp20NGroupsGroupIdDrivesDriveIdItemsDriveitemIdMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action createUploadSession

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

To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPathsPpp20NGroupsGroupIdDrivesDriveIdItemsDriveitemIdMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema
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

### -DriveId
The unique identifier of drive

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

### -DriveItemId
The unique identifier of driveItem

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IFilesIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Item
driveItemUploadableProperties
To construct, see NOTES section for ITEM properties and create a hash table.

```yaml
Type: IMicrosoftGraphDriveItemUploadableProperties
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
### Microsoft.Graph.Beta.PowerShell.Models.IPathsPpp20NGroupsGroupIdDrivesDriveIdItemsDriveitemIdMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUploadSession
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsPpp20NGroupsGroupIdDrivesDriveIdItemsDriveitemIdMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Item <IMicrosoftGraphDriveItemUploadableProperties>]`: driveItemUploadableProperties
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Description <String>]`: Provides a user-visible description of the item.
Read-write.
Only on OneDrive Personal.
    - `[DriveItemSource <IMicrosoftGraphDriveItemSource>]`: driveItemSource
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <String>]`: driveItemSourceApplication
      - `[ExternalId <String>]`: The external identifier for the drive item from the source.
    - `[FileSize <Int64?>]`: Provides an expected file size to perform a quota check prior to upload.
Only on OneDrive Personal.
    - `[FileSystemInfo <IMicrosoftGraphFileSystemInfo>]`: fileSystemInfo
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CreatedDateTime <DateTime?>]`: The UTC date and time the file was created on a client.
      - `[LastAccessedDateTime <DateTime?>]`: The UTC date and time the file was last accessed.
Available for the recent file list only.
      - `[LastModifiedDateTime <DateTime?>]`: The UTC date and time the file was last modified on a client.
    - `[MediaSource <IMicrosoftGraphMediaSource>]`: mediaSource
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ContentCategory <String>]`: mediaSourceContentCategory
    - `[Name <String>]`: The name of the item (filename and extension).
Read-write.

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

ITEM `<IMicrosoftGraphDriveItemUploadableProperties>`: driveItemUploadableProperties
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Description <String>]`: Provides a user-visible description of the item.
Read-write.
Only on OneDrive Personal.
  - `[DriveItemSource <IMicrosoftGraphDriveItemSource>]`: driveItemSource
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <String>]`: driveItemSourceApplication
    - `[ExternalId <String>]`: The external identifier for the drive item from the source.
  - `[FileSize <Int64?>]`: Provides an expected file size to perform a quota check prior to upload.
Only on OneDrive Personal.
  - `[FileSystemInfo <IMicrosoftGraphFileSystemInfo>]`: fileSystemInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CreatedDateTime <DateTime?>]`: The UTC date and time the file was created on a client.
    - `[LastAccessedDateTime <DateTime?>]`: The UTC date and time the file was last accessed.
Available for the recent file list only.
    - `[LastModifiedDateTime <DateTime?>]`: The UTC date and time the file was last modified on a client.
  - `[MediaSource <IMicrosoftGraphMediaSource>]`: mediaSource
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ContentCategory <String>]`: mediaSourceContentCategory
  - `[Name <String>]`: The name of the item (filename and extension).
Read-write.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.files/new-mgbetagroupdriveitemuploadsession](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.files/new-mgbetagroupdriveitemuploadsession)
























