---
external help file: Microsoft.Graph.Users-help.xml
Module Name: Microsoft.Graph.Users
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users/update-mgusersettingshiftpreference
schema: 2.0.0
ms.subservice: teams
---

# Update-MgUserSettingShiftPreference

## SYNOPSIS
Update the properties and relationships of a shiftPreferences object.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaUserSettingShiftPreference](/powershell/module/Microsoft.Graph.Beta.Users/Update-MgBetaUserSettingShiftPreference?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgUserSettingShiftPreference -UserId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Availability <IMicrosoftGraphShiftAvailability[]>]
 [-CreatedBy <IMicrosoftGraphIdentitySet>] [-Id <String>] [-LastModifiedBy <IMicrosoftGraphIdentitySet>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgUserSettingShiftPreference -UserId <String> -BodyParameter <IMicrosoftGraphShiftPreferences>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgUserSettingShiftPreference -InputObject <IUsersIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Availability <IMicrosoftGraphShiftAvailability[]>]
 [-CreatedBy <IMicrosoftGraphIdentitySet>] [-Id <String>] [-LastModifiedBy <IMicrosoftGraphIdentitySet>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgUserSettingShiftPreference -InputObject <IUsersIdentity>
 -BodyParameter <IMicrosoftGraphShiftPreferences> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties and relationships of a shiftPreferences object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | User.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | UserShiftPreferences.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Users

$params = @{
	id = "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7"
	"@odata.etag" = "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa"
	availability = @(
		@{
			recurrence = @{
				pattern = @{
					type = "Weekly"
					daysOfWeek = @(
					"Monday"
				"Wednesday"
			"Friday"
		)
		interval = 1
	}
	range = @{
		type = "noEnd"
	}
}
timeZone = "Pacific Standard Time"
timeSlots = $null
}
)
}

Update-MgUserSettingShiftPreference -UserId $userId -BodyParameter $params

```
This example shows how to use the Update-MgUserSettingShiftPreference Cmdlet.


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

### -Availability
Availability of the user to be scheduled for work and its recurrence pattern.
To construct, see NOTES section for AVAILABILITY properties and create a hash table.

```yaml
Type: IMicrosoftGraphShiftAvailability[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
shiftPreferences
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphShiftPreferences
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

### -CreatedBy
identitySet
To construct, see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
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

### -LastModifiedBy
identitySet
To construct, see NOTES section for LASTMODIFIEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphShiftPreferences
### Microsoft.Graph.PowerShell.Models.IUsersIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphShiftPreferences
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

AVAILABILITY `<IMicrosoftGraphShiftAvailability- `[]`>`: Availability of the user to be scheduled for work and its recurrence pattern.
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
  - `[TimeSlots <IMicrosoftGraphTimeRange- `[]`>]`: The time slot(s) preferred by the user.
    - `[EndTime <String>]`: End time for the time range.
    - `[StartTime <String>]`: Start time for the time range.
  - `[TimeZone <String>]`: Specifies the time zone for the indicated time.

BODYPARAMETER `<IMicrosoftGraphShiftPreferences>`: shiftPreferences
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
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
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Availability <IMicrosoftGraphShiftAvailability- `[]`>]`: Availability of the user to be scheduled for work and its recurrence pattern.
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
    - `[TimeSlots <IMicrosoftGraphTimeRange- `[]`>]`: The time slot(s) preferred by the user.
      - `[EndTime <String>]`: End time for the time range.
      - `[StartTime <String>]`: Start time for the time range.
    - `[TimeZone <String>]`: Specifies the time zone for the indicated time.

CREATEDBY `<IMicrosoftGraphIdentitySet>`: identitySet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Application <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
    - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
  - `[Device <IMicrosoftGraphIdentity>]`: identity
  - `[User <IMicrosoftGraphIdentity>]`: identity

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

LASTMODIFIEDBY `<IMicrosoftGraphIdentitySet>`: identitySet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Application <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
    - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
  - `[Device <IMicrosoftGraphIdentity>]`: identity
  - `[User <IMicrosoftGraphIdentity>]`: identity

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.users/update-mgusersettingshiftpreference](https://learn.microsoft.com/powershell/module/microsoft.graph.users/update-mgusersettingshiftpreference)

[https://learn.microsoft.com/graph/api/shiftpreferences-put?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/shiftpreferences-put?view=graph-rest-1.0)























