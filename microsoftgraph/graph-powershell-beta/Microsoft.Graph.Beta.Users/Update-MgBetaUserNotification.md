---
external help file: Microsoft.Graph.Beta.Users-help.xml
Module Name: Microsoft.Graph.Beta.Users
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users/update-mgbetausernotification
schema: 2.0.0
---

# Update-MgBetaUserNotification

## SYNOPSIS
Update the navigation property notifications in users

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaUserNotification -NotificationId <String> -UserId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-DisplayTimeToLive <Int32>] [-ExpirationDateTime <DateTime>]
 [-GroupName <String>] [-Id <String>] [-Payload <IMicrosoftGraphPayloadTypes>] [-Priority <String>]
 [-TargetHostName <String>] [-TargetPolicy <IMicrosoftGraphTargetPolicyEndpoints>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaUserNotification -NotificationId <String> -UserId <String>
 -BodyParameter <IMicrosoftGraphNotification> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaUserNotification -InputObject <IUsersIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-DisplayTimeToLive <Int32>] [-ExpirationDateTime <DateTime>]
 [-GroupName <String>] [-Id <String>] [-Payload <IMicrosoftGraphPayloadTypes>] [-Priority <String>]
 [-TargetHostName <String>] [-TargetPolicy <IMicrosoftGraphTargetPolicyEndpoints>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaUserNotification -InputObject <IUsersIdentity> -BodyParameter <IMicrosoftGraphNotification>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property notifications in users

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
notification
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphNotification
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

### -DisplayTimeToLive
Sets how long (in seconds) this notification content stays in each platform's notification viewer.
For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification stays in the user's Windows Action Center.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpirationDateTime
Sets a UTC expiration date and time on a user notification using ISO 8601 format (for example, midnight UTC on Jan 1, 2019 would look like this: '2019-01-01T00:00:00Z').
When time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.
Max value is 30 days.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupName
The name of the group that this notification belongs to.
It is set by the developer for grouping notifications together.

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
Type: IUsersIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NotificationId
The unique identifier of notification

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

### -Payload
payloadTypes
To construct, see NOTES section for PAYLOAD properties and create a hash table.

```yaml
Type: IMicrosoftGraphPayloadTypes
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Priority
priority

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

### -TargetHostName
Represents the host name of the app to which the calling service wants to post the notification, for the given user.
If targeting web endpoints (see targetPolicy.platformTypes), ensure that targetHostName is the same as the name used when creating a subscription on the client side within the application JSON property.

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

### -TargetPolicy
targetPolicyEndpoints
To construct, see NOTES section for TARGETPOLICY properties and create a hash table.

```yaml
Type: IMicrosoftGraphTargetPolicyEndpoints
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphNotification
### Microsoft.Graph.Beta.PowerShell.Models.IUsersIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphNotification
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphNotification>`: notification
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayTimeToLive <Int32?>]`: Sets how long (in seconds) this notification content stays in each platform's notification viewer.
For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification stays in the user's Windows Action Center.
  - `[ExpirationDateTime <DateTime?>]`: Sets a UTC expiration date and time on a user notification using ISO 8601 format (for example, midnight UTC on Jan 1, 2019 would look like this: '2019-01-01T00:00:00Z').
When time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.
Max value is 30 days.
  - `[GroupName <String>]`: The name of the group that this notification belongs to.
It is set by the developer for grouping notifications together.
  - `[Payload <IMicrosoftGraphPayloadTypes>]`: payloadTypes
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[RawContent <String>]`: The notification content of a raw user notification that will be delivered to and consumed by the app client on all supported platforms (Windows, iOS, Android or WebPush) receiving this notification.
At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.
    - `[VisualContent <IMicrosoftGraphVisualProperties>]`: visualProperties
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Body <String>]`: The body of a visual user notification.
Body is optional.
      - `[Title <String>]`: The title of a visual user notification.
This field is required for visual notification payloads.
  - `[Priority <String>]`: priority
  - `[TargetHostName <String>]`: Represents the host name of the app to which the calling service wants to post the notification, for the given user.
If targeting web endpoints (see targetPolicy.platformTypes), ensure that targetHostName is the same as the name used when creating a subscription on the client side within the application JSON property.
  - `[TargetPolicy <IMicrosoftGraphTargetPolicyEndpoints>]`: targetPolicyEndpoints
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[PlatformTypes <String- `[]`>]`: Use to filter the notification distribution to a specific platform or platforms.
Valid values are Windows, iOS, Android and WebPush.
By default, all push endpoint types (Windows, iOS, Android and WebPush) are enabled.

INPUTOBJECT `<IUsersIdentity>`: Identity Parameter
  - `[AppId <String>]`: Alternate key of servicePrincipal
  - `[AttachmentBaseId <String>]`: The unique identifier of attachmentBase
  - `[AttachmentId <String>]`: The unique identifier of attachment
  - `[AttachmentSessionId <String>]`: The unique identifier of attachmentSession
  - `[ChecklistItemId <String>]`: The unique identifier of checklistItem
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[LicenseDetailsId <String>]`: The unique identifier of licenseDetails
  - `[LinkedResourceId <String>]`: The unique identifier of linkedResource
  - `[NotificationId <String>]`: The unique identifier of notification
  - `[OAuth2PermissionGrantId <String>]`: The unique identifier of oAuth2PermissionGrant
  - `[OutlookCategoryId <String>]`: The unique identifier of outlookCategory
  - `[OutlookTaskFolderId <String>]`: The unique identifier of outlookTaskFolder
  - `[OutlookTaskGroupId <String>]`: The unique identifier of outlookTaskGroup
  - `[OutlookTaskId <String>]`: The unique identifier of outlookTask
  - `[ProfilePhotoId <String>]`: The unique identifier of profilePhoto
  - `[ServicePrincipalId <String>]`: The unique identifier of servicePrincipal
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

PAYLOAD `<IMicrosoftGraphPayloadTypes>`: payloadTypes
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[RawContent <String>]`: The notification content of a raw user notification that will be delivered to and consumed by the app client on all supported platforms (Windows, iOS, Android or WebPush) receiving this notification.
At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.
  - `[VisualContent <IMicrosoftGraphVisualProperties>]`: visualProperties
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Body <String>]`: The body of a visual user notification.
Body is optional.
    - `[Title <String>]`: The title of a visual user notification.
This field is required for visual notification payloads.

TARGETPOLICY `<IMicrosoftGraphTargetPolicyEndpoints>`: targetPolicyEndpoints
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[PlatformTypes <String- `[]`>]`: Use to filter the notification distribution to a specific platform or platforms.
Valid values are Windows, iOS, Android and WebPush.
By default, all push endpoint types (Windows, iOS, Android and WebPush) are enabled.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users/update-mgbetausernotification](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users/update-mgbetausernotification)
























