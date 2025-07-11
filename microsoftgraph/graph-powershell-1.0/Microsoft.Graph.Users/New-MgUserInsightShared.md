---
external help file: Microsoft.Graph.Users-help.xml
Module Name: Microsoft.Graph.Users
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users/new-mguserinsightshared
schema: 2.0.0
---

# New-MgUserInsightShared

## SYNOPSIS
Create new navigation property to shared for users

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaUserInsightShared](/powershell/module/Microsoft.Graph.Beta.Users/New-MgBetaUserInsightShared?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgUserInsightShared -UserId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Id <String>] [-LastShared <IMicrosoftGraphSharingDetail>]
 [-LastSharedMethod <IMicrosoftGraphEntity>] [-Resource <IMicrosoftGraphEntity>]
 [-ResourceReference <IMicrosoftGraphResourceReference>]
 [-ResourceVisualization <IMicrosoftGraphResourceVisualization>]
 [-SharingHistory <IMicrosoftGraphSharingDetail[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgUserInsightShared -UserId <String> -BodyParameter <IMicrosoftGraphSharedInsight>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgUserInsightShared -InputObject <IUsersIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Id <String>] [-LastShared <IMicrosoftGraphSharingDetail>]
 [-LastSharedMethod <IMicrosoftGraphEntity>] [-Resource <IMicrosoftGraphEntity>]
 [-ResourceReference <IMicrosoftGraphResourceReference>]
 [-ResourceVisualization <IMicrosoftGraphResourceVisualization>]
 [-SharingHistory <IMicrosoftGraphSharingDetail[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgUserInsightShared -InputObject <IUsersIdentity> -BodyParameter <IMicrosoftGraphSharedInsight>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to shared for users

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
sharedInsight
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSharedInsight
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
Type: IUsersIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LastShared
sharingDetail
To construct, see NOTES section for LASTSHARED properties and create a hash table.

```yaml
Type: IMicrosoftGraphSharingDetail
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastSharedMethod
entity
To construct, see NOTES section for LASTSHAREDMETHOD properties and create a hash table.

```yaml
Type: IMicrosoftGraphEntity
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Resource
entity
To construct, see NOTES section for RESOURCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphEntity
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceReference
resourceReference
To construct, see NOTES section for RESOURCEREFERENCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphResourceReference
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceVisualization
resourceVisualization
To construct, see NOTES section for RESOURCEVISUALIZATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphResourceVisualization
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

### -SharingHistory

To construct, see NOTES section for SHARINGHISTORY properties and create a hash table.

```yaml
Type: IMicrosoftGraphSharingDetail[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
The unique identifier of user

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphSharedInsight
### Microsoft.Graph.PowerShell.Models.IUsersIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphSharedInsight
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphSharedInsight>`: sharedInsight
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[LastShared <IMicrosoftGraphSharingDetail>]`: sharingDetail
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[SharedBy <IMicrosoftGraphInsightIdentity>]`: insightIdentity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Address <String>]`: The email address of the user who shared the item.
      - `[DisplayName <String>]`: The display name of the user who shared the item.
      - `[Id <String>]`: The ID of the user who shared the item.
    - `[SharedDateTime <DateTime?>]`: The date and time the file was last shared.
The timestamp represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    - `[SharingReference <IMicrosoftGraphResourceReference>]`: resourceReference
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The item's unique identifier.
      - `[Type <String>]`: A string value that can be used to classify the item, such as 'microsoft.graph.driveItem'
      - `[WebUrl <String>]`: A URL leading to the referenced item.
    - `[SharingSubject <String>]`: The subject with which the document was shared.
    - `[SharingType <String>]`: Determines the way the document was shared.
Can be by a 1Link1, 1Attachment1, 1Group1, 1Site1.
  - `[LastSharedMethod <IMicrosoftGraphEntity>]`: entity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Resource <IMicrosoftGraphEntity>]`: entity
  - `[ResourceReference <IMicrosoftGraphResourceReference>]`: resourceReference
  - `[ResourceVisualization <IMicrosoftGraphResourceVisualization>]`: resourceVisualization
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ContainerDisplayName <String>]`: A string describing where the item is stored.
For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.
    - `[ContainerType <String>]`: Can be used for filtering by the type of container in which the file is stored.
Such as Site or OneDriveBusiness.
    - `[ContainerWebUrl <String>]`: A path leading to the folder in which the item is stored.
    - `[MediaType <String>]`: The item's media type.
Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.
Not all Media Mime Types are supported.
    - `[PreviewImageUrl <String>]`: A URL leading to the preview image for the item.
    - `[PreviewText <String>]`: A preview text for the item.
    - `[Title <String>]`: The item's title text.
    - `[Type <String>]`: The item's media type.
Can be used for filtering for a specific file based on a specific type.
See the section Type property values for supported types.
  - `[SharingHistory <IMicrosoftGraphSharingDetail- `[]`>]`:

INPUTOBJECT `<IUsersIdentity>`: Identity Parameter
  - `[AttachmentBaseId <String>]`: The unique identifier of attachmentBase
  - `[AttachmentSessionId <String>]`: The unique identifier of attachmentSession
  - `[ChecklistItemId <String>]`: The unique identifier of checklistItem
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[LicenseDetailsId <String>]`: The unique identifier of licenseDetails
  - `[LinkedResourceId <String>]`: The unique identifier of linkedResource
  - `[OAuth2PermissionGrantId <String>]`: The unique identifier of oAuth2PermissionGrant
  - `[OutlookCategoryId <String>]`: The unique identifier of outlookCategory
  - `[ProfilePhotoId <String>]`: The unique identifier of profilePhoto
  - `[ServiceStorageQuotaBreakdownId <String>]`: The unique identifier of serviceStorageQuotaBreakdown
  - `[SharedInsightId <String>]`: The unique identifier of sharedInsight
  - `[TimeZoneStandard <String>]`: Usage: TimeZoneStandard='{TimeZoneStandard}'
  - `[TodoTaskId <String>]`: The unique identifier of todoTask
  - `[TodoTaskListId <String>]`: The unique identifier of todoTaskList
  - `[TrendingId <String>]`: The unique identifier of trending
  - `[UsedInsightId <String>]`: The unique identifier of usedInsight
  - `[UserId <String>]`: The unique identifier of user
  - `[UserPrincipalName <String>]`: Alternate key of user
  - `[WindowsSettingId <String>]`: The unique identifier of windowsSetting
  - `[WindowsSettingInstanceId <String>]`: The unique identifier of windowsSettingInstance

LASTSHARED `<IMicrosoftGraphSharingDetail>`: sharingDetail
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[SharedBy <IMicrosoftGraphInsightIdentity>]`: insightIdentity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Address <String>]`: The email address of the user who shared the item.
    - `[DisplayName <String>]`: The display name of the user who shared the item.
    - `[Id <String>]`: The ID of the user who shared the item.
  - `[SharedDateTime <DateTime?>]`: The date and time the file was last shared.
The timestamp represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
  - `[SharingReference <IMicrosoftGraphResourceReference>]`: resourceReference
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The item's unique identifier.
    - `[Type <String>]`: A string value that can be used to classify the item, such as 'microsoft.graph.driveItem'
    - `[WebUrl <String>]`: A URL leading to the referenced item.
  - `[SharingSubject <String>]`: The subject with which the document was shared.
  - `[SharingType <String>]`: Determines the way the document was shared.
Can be by a 1Link1, 1Attachment1, 1Group1, 1Site1.

LASTSHAREDMETHOD `<IMicrosoftGraphEntity>`: entity
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

RESOURCE `<IMicrosoftGraphEntity>`: entity
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

RESOURCEREFERENCE `<IMicrosoftGraphResourceReference>`: resourceReference
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The item's unique identifier.
  - `[Type <String>]`: A string value that can be used to classify the item, such as 'microsoft.graph.driveItem'
  - `[WebUrl <String>]`: A URL leading to the referenced item.

RESOURCEVISUALIZATION `<IMicrosoftGraphResourceVisualization>`: resourceVisualization
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ContainerDisplayName <String>]`: A string describing where the item is stored.
For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.
  - `[ContainerType <String>]`: Can be used for filtering by the type of container in which the file is stored.
Such as Site or OneDriveBusiness.
  - `[ContainerWebUrl <String>]`: A path leading to the folder in which the item is stored.
  - `[MediaType <String>]`: The item's media type.
Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.
Not all Media Mime Types are supported.
  - `[PreviewImageUrl <String>]`: A URL leading to the preview image for the item.
  - `[PreviewText <String>]`: A preview text for the item.
  - `[Title <String>]`: The item's title text.
  - `[Type <String>]`: The item's media type.
Can be used for filtering for a specific file based on a specific type.
See the section Type property values for supported types.

SHARINGHISTORY `<IMicrosoftGraphSharingDetail- `[]`>`: .
  - `[SharedBy <IMicrosoftGraphInsightIdentity>]`: insightIdentity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Address <String>]`: The email address of the user who shared the item.
    - `[DisplayName <String>]`: The display name of the user who shared the item.
    - `[Id <String>]`: The ID of the user who shared the item.
  - `[SharedDateTime <DateTime?>]`: The date and time the file was last shared.
The timestamp represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
  - `[SharingReference <IMicrosoftGraphResourceReference>]`: resourceReference
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The item's unique identifier.
    - `[Type <String>]`: A string value that can be used to classify the item, such as 'microsoft.graph.driveItem'
    - `[WebUrl <String>]`: A URL leading to the referenced item.
  - `[SharingSubject <String>]`: The subject with which the document was shared.
  - `[SharingType <String>]`: Determines the way the document was shared.
Can be by a 1Link1, 1Attachment1, 1Group1, 1Site1.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.users/new-mguserinsightshared](https://learn.microsoft.com/powershell/module/microsoft.graph.users/new-mguserinsightshared)
























