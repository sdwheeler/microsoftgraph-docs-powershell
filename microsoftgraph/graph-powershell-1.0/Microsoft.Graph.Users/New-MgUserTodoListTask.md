---
external help file: Microsoft.Graph.Users-help.xml
Module Name: Microsoft.Graph.Users
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users/new-mgusertodolisttask
schema: 2.0.0
---

# New-MgUserTodoListTask

## SYNOPSIS
Create new navigation property to tasks for users

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaUserTodoListTask](/powershell/module/Microsoft.Graph.Beta.Users/New-MgBetaUserTodoListTask?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgUserTodoListTask -TodoTaskListId <String> -UserId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AttachmentSessions <IMicrosoftGraphAttachmentSession[]>]
 [-Attachments <IMicrosoftGraphAttachmentBase[]>] [-Body <IMicrosoftGraphItemBody>]
 [-BodyLastModifiedDateTime <DateTime>] [-Categories <String[]>]
 [-ChecklistItems <IMicrosoftGraphChecklistItem[]>] [-CompletedDateTime <IMicrosoftGraphDateTimeZone>]
 [-CreatedDateTime <DateTime>] [-DueDateTime <IMicrosoftGraphDateTimeZone>]
 [-Extensions <IMicrosoftGraphExtension[]>] [-HasAttachments] [-Id <String>] [-Importance <String>]
 [-IsReminderOn] [-LastModifiedDateTime <DateTime>] [-LinkedResources <IMicrosoftGraphLinkedResource[]>]
 [-Recurrence <IMicrosoftGraphPatternedRecurrence>] [-ReminderDateTime <IMicrosoftGraphDateTimeZone>]
 [-StartDateTime <IMicrosoftGraphDateTimeZone>] [-Status <String>] [-Title <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgUserTodoListTask -TodoTaskListId <String> -UserId <String> -BodyParameter <IMicrosoftGraphTodoTask>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgUserTodoListTask -InputObject <IUsersIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AttachmentSessions <IMicrosoftGraphAttachmentSession[]>]
 [-Attachments <IMicrosoftGraphAttachmentBase[]>] [-Body <IMicrosoftGraphItemBody>]
 [-BodyLastModifiedDateTime <DateTime>] [-Categories <String[]>]
 [-ChecklistItems <IMicrosoftGraphChecklistItem[]>] [-CompletedDateTime <IMicrosoftGraphDateTimeZone>]
 [-CreatedDateTime <DateTime>] [-DueDateTime <IMicrosoftGraphDateTimeZone>]
 [-Extensions <IMicrosoftGraphExtension[]>] [-HasAttachments] [-Id <String>] [-Importance <String>]
 [-IsReminderOn] [-LastModifiedDateTime <DateTime>] [-LinkedResources <IMicrosoftGraphLinkedResource[]>]
 [-Recurrence <IMicrosoftGraphPatternedRecurrence>] [-ReminderDateTime <IMicrosoftGraphDateTimeZone>]
 [-StartDateTime <IMicrosoftGraphDateTimeZone>] [-Status <String>] [-Title <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgUserTodoListTask -InputObject <IUsersIdentity> -BodyParameter <IMicrosoftGraphTodoTask>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to tasks for users

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Tasks.ReadWrite,  |
| Delegated (personal Microsoft account) | Tasks.ReadWrite,  |
| Application | Tasks.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.Users

$params = @{
	title = "A new task"
	categories = @(
		"Important"
	)
	linkedResources = @(
		@{
			webUrl = "http://microsoft.com"
			applicationName = "Microsoft"
			displayName = "Microsoft"
		}
	)
}

# A UPN can also be used as -UserId.
New-MgUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId -BodyParameter $params
```
This example shows how to use the New-MgUserTodoListTask Cmdlet.

To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


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

### -Attachments
A collection of file attachments for the task.
To construct, see NOTES section for ATTACHMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAttachmentBase[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AttachmentSessions

To construct, see NOTES section for ATTACHMENTSESSIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAttachmentSession[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Body
itemBody
To construct, see NOTES section for BODY properties and create a hash table.

```yaml
Type: IMicrosoftGraphItemBody
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyLastModifiedDateTime
The date and time when the task body was last modified.
By default, it is in UTC.
You can provide a custom time zone in the request header.
The property value uses ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
todoTask
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTodoTask
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Categories
The categories associated with the task.
Each category corresponds to the displayName property of an outlookCategory that the user has defined.

```yaml
Type: String[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ChecklistItems
A collection of checklistItems linked to a task.
To construct, see NOTES section for CHECKLISTITEMS properties and create a hash table.

```yaml
Type: IMicrosoftGraphChecklistItem[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CompletedDateTime
dateTimeTimeZone
To construct, see NOTES section for COMPLETEDDATETIME properties and create a hash table.

```yaml
Type: IMicrosoftGraphDateTimeZone
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### -CreatedDateTime
The date and time when the task was created.
By default, it is in UTC.
You can provide a custom time zone in the request header.
The property value uses ISO 8601 format.
For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DueDateTime
dateTimeTimeZone
To construct, see NOTES section for DUEDATETIME properties and create a hash table.

```yaml
Type: IMicrosoftGraphDateTimeZone
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Extensions
The collection of open extensions defined for the task.
Nullable.
To construct, see NOTES section for EXTENSIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphExtension[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HasAttachments
Indicates whether the task has attachments.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
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

### -Importance
importance

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

### -IsReminderOn
Set to true if an alert is set to remind the user of the task.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
The date and time when the task was last modified.
By default, it is in UTC.
You can provide a custom time zone in the request header.
The property value uses ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LinkedResources
A collection of resources linked to the task.
To construct, see NOTES section for LINKEDRESOURCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphLinkedResource[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Recurrence
patternedRecurrence
To construct, see NOTES section for RECURRENCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphPatternedRecurrence
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReminderDateTime
dateTimeTimeZone
To construct, see NOTES section for REMINDERDATETIME properties and create a hash table.

```yaml
Type: IMicrosoftGraphDateTimeZone
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

### -StartDateTime
dateTimeTimeZone
To construct, see NOTES section for STARTDATETIME properties and create a hash table.

```yaml
Type: IMicrosoftGraphDateTimeZone
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
taskStatus

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

### -Title
A brief description of the task.

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

### -TodoTaskListId
The unique identifier of todoTaskList

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTodoTask
### Microsoft.Graph.PowerShell.Models.IUsersIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTodoTask
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ATTACHMENTS `<IMicrosoftGraphAttachmentBase- `[]`>`: A collection of file attachments for the task.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ContentType <String>]`: The MIME type.
  - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[Name <String>]`: The display name of the attachment.
This doesn't need to be the actual file name.
  - `[Size <Int32?>]`: The length of the attachment in bytes.

ATTACHMENTSESSIONS `<IMicrosoftGraphAttachmentSession- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Content <Byte- `[]`>]`: The content streams that are uploaded.
  - `[ExpirationDateTime <DateTime?>]`: The date and time in UTC when the upload session will expire.
The complete file must be uploaded before this expiration time is reached.
  - `[NextExpectedRanges <String- `[]`>]`: Indicates a single value {start} that represents the location in the file where the next upload should begin.

BODY `<IMicrosoftGraphItemBody>`: itemBody
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Content <String>]`: The content of the item.
  - `[ContentType <String>]`: bodyType

BODYPARAMETER `<IMicrosoftGraphTodoTask>`: todoTask
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AttachmentSessions <IMicrosoftGraphAttachmentSession- `[]`>]`:
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Content <Byte- `[]`>]`: The content streams that are uploaded.
    - `[ExpirationDateTime <DateTime?>]`: The date and time in UTC when the upload session will expire.
The complete file must be uploaded before this expiration time is reached.
    - `[NextExpectedRanges <String- `[]`>]`: Indicates a single value {start} that represents the location in the file where the next upload should begin.
  - `[Attachments <IMicrosoftGraphAttachmentBase- `[]`>]`: A collection of file attachments for the task.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ContentType <String>]`: The MIME type.
    - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[Name <String>]`: The display name of the attachment.
This doesn't need to be the actual file name.
    - `[Size <Int32?>]`: The length of the attachment in bytes.
  - `[Body <IMicrosoftGraphItemBody>]`: itemBody
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Content <String>]`: The content of the item.
    - `[ContentType <String>]`: bodyType
  - `[BodyLastModifiedDateTime <DateTime?>]`: The date and time when the task body was last modified.
By default, it is in UTC.
You can provide a custom time zone in the request header.
The property value uses ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.
  - `[Categories <String- `[]`>]`: The categories associated with the task.
Each category corresponds to the displayName property of an outlookCategory that the user has defined.
  - `[ChecklistItems <IMicrosoftGraphChecklistItem- `[]`>]`: A collection of checklistItems linked to a task.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CheckedDateTime <DateTime?>]`: The date and time when the checklistItem was finished.
    - `[CreatedDateTime <DateTime?>]`: The date and time when the checklistItem was created.
    - `[DisplayName <String>]`: Indicates the title of the checklistItem.
    - `[IsChecked <Boolean?>]`: State that indicates whether the item is checked off or not.
  - `[CompletedDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
    - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for more possible values.
  - `[CreatedDateTime <DateTime?>]`: The date and time when the task was created.
By default, it is in UTC.
You can provide a custom time zone in the request header.
The property value uses ISO 8601 format.
For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.
  - `[DueDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
  - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the task.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[HasAttachments <Boolean?>]`: Indicates whether the task has attachments.
  - `[Importance <String>]`: importance
  - `[IsReminderOn <Boolean?>]`: Set to true if an alert is set to remind the user of the task.
  - `[LastModifiedDateTime <DateTime?>]`: The date and time when the task was last modified.
By default, it is in UTC.
You can provide a custom time zone in the request header.
The property value uses ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.
  - `[LinkedResources <IMicrosoftGraphLinkedResource- `[]`>]`: A collection of resources linked to the task.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ApplicationName <String>]`: The app name of the source that sends the linkedResource.
    - `[DisplayName <String>]`: The title of the linkedResource.
    - `[ExternalId <String>]`: ID of the object that is associated with this task on the third-party/partner system.
    - `[WebUrl <String>]`: Deep link to the linkedResource.
  - `[Recurrence <IMicrosoftGraphPatternedRecurrence>]`: patternedRecurrence
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Pattern <IMicrosoftGraphRecurrencePattern>]`: recurrencePattern
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DayOfMonth <Int32?>]`: The day of the month on which the event occurs.
Required if type is absoluteMonthly or absoluteYearly.
      - `[DaysOfWeek <String- `[]`>]`: A collection of the days of the week on which the event occurs.
The possible values are: sunday, monday, tuesday, wednesday, thursday, friday, saturday.
If type is relativeMonthly or relativeYearly, and daysOfWeek specifies more than one day, the event falls on the first day that satisfies the pattern.
Required if type is weekly, relativeMonthly, or relativeYearly.
      - `[FirstDayOfWeek <String>]`: dayOfWeek
      - `[Index <String>]`: weekIndex
      - `[Interval <Int32?>]`: The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the type.
Required.
      - `[Month <Int32?>]`: The month in which the event occurs.
This is a number from 1 to 12.
      - `[Type <String>]`: recurrencePatternType
    - `[Range <IMicrosoftGraphRecurrenceRange>]`: recurrenceRange
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[EndDate <DateTime?>]`: The date to stop applying the recurrence pattern.
Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.
Required if type is endDate.
      - `[NumberOfOccurrences <Int32?>]`: The number of times to repeat the event.
Required and must be positive if type is numbered.
      - `[RecurrenceTimeZone <String>]`: Time zone for the startDate and endDate properties.
Optional.
If not specified, the time zone of the event is used.
      - `[StartDate <DateTime?>]`: The date to start applying the recurrence pattern.
The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.
Must be the same value as the start property of the recurring event.
Required.
      - `[Type <String>]`: recurrenceRangeType
  - `[ReminderDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
  - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
  - `[Status <String>]`: taskStatus
  - `[Title <String>]`: A brief description of the task.

CHECKLISTITEMS `<IMicrosoftGraphChecklistItem- `[]`>`: A collection of checklistItems linked to a task.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CheckedDateTime <DateTime?>]`: The date and time when the checklistItem was finished.
  - `[CreatedDateTime <DateTime?>]`: The date and time when the checklistItem was created.
  - `[DisplayName <String>]`: Indicates the title of the checklistItem.
  - `[IsChecked <Boolean?>]`: State that indicates whether the item is checked off or not.

COMPLETEDDATETIME `<IMicrosoftGraphDateTimeZone>`: dateTimeTimeZone
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
  - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for more possible values.

DUEDATETIME `<IMicrosoftGraphDateTimeZone>`: dateTimeTimeZone
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
  - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for more possible values.

EXTENSIONS `<IMicrosoftGraphExtension- `[]`>`: The collection of open extensions defined for the task.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

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

LINKEDRESOURCES `<IMicrosoftGraphLinkedResource- `[]`>`: A collection of resources linked to the task.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ApplicationName <String>]`: The app name of the source that sends the linkedResource.
  - `[DisplayName <String>]`: The title of the linkedResource.
  - `[ExternalId <String>]`: ID of the object that is associated with this task on the third-party/partner system.
  - `[WebUrl <String>]`: Deep link to the linkedResource.

RECURRENCE `<IMicrosoftGraphPatternedRecurrence>`: patternedRecurrence
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Pattern <IMicrosoftGraphRecurrencePattern>]`: recurrencePattern
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DayOfMonth <Int32?>]`: The day of the month on which the event occurs.
Required if type is absoluteMonthly or absoluteYearly.
    - `[DaysOfWeek <String- `[]`>]`: A collection of the days of the week on which the event occurs.
The possible values are: sunday, monday, tuesday, wednesday, thursday, friday, saturday.
If type is relativeMonthly or relativeYearly, and daysOfWeek specifies more than one day, the event falls on the first day that satisfies the pattern.
Required if type is weekly, relativeMonthly, or relativeYearly.
    - `[FirstDayOfWeek <String>]`: dayOfWeek
    - `[Index <String>]`: weekIndex
    - `[Interval <Int32?>]`: The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the type.
Required.
    - `[Month <Int32?>]`: The month in which the event occurs.
This is a number from 1 to 12.
    - `[Type <String>]`: recurrencePatternType
  - `[Range <IMicrosoftGraphRecurrenceRange>]`: recurrenceRange
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[EndDate <DateTime?>]`: The date to stop applying the recurrence pattern.
Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.
Required if type is endDate.
    - `[NumberOfOccurrences <Int32?>]`: The number of times to repeat the event.
Required and must be positive if type is numbered.
    - `[RecurrenceTimeZone <String>]`: Time zone for the startDate and endDate properties.
Optional.
If not specified, the time zone of the event is used.
    - `[StartDate <DateTime?>]`: The date to start applying the recurrence pattern.
The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.
Must be the same value as the start property of the recurring event.
Required.
    - `[Type <String>]`: recurrenceRangeType

REMINDERDATETIME `<IMicrosoftGraphDateTimeZone>`: dateTimeTimeZone
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
  - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for more possible values.

STARTDATETIME `<IMicrosoftGraphDateTimeZone>`: dateTimeTimeZone
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
  - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for more possible values.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.users/new-mgusertodolisttask](https://learn.microsoft.com/powershell/module/microsoft.graph.users/new-mgusertodolisttask)























