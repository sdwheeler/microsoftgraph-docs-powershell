---
external help file: Microsoft.Graph.Users-help.xml
Module Name: Microsoft.Graph.Users
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users/get-mgusersettingiteminsight
schema: 2.0.0
---

# Get-MgUserSettingItemInsight

## SYNOPSIS
The user's settings for the visibility of meeting hour insights, and insights derived between a user and other items in Microsoft 365, such as documents or sites.
Get userInsightsSettings through this navigation property.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaUserSettingItemInsight](/powershell/module/Microsoft.Graph.Beta.Users/Get-MgBetaUserSettingItemInsight?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgUserSettingItemInsight -UserId <String> [-ExpandProperty <String[]>] [-Property <String[]>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgUserSettingItemInsight -InputObject <IUsersIdentity> [-ExpandProperty <String[]>] [-Property <String[]>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
The user's settings for the visibility of meeting hour insights, and insights derived between a user and other items in Microsoft 365, such as documents or sites.
Get userInsightsSettings through this navigation property.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | User.Read, User.ReadWrite,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Not supported |

## EXAMPLES

## PARAMETERS

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Expand

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IUsersIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

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

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IUsersIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUserInsightsSettings
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.users/get-mgusersettingiteminsight](https://learn.microsoft.com/powershell/module/microsoft.graph.users/get-mgusersettingiteminsight)
























