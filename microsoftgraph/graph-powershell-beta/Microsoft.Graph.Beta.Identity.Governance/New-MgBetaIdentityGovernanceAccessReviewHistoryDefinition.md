---
external help file: Microsoft.Graph.Beta.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Beta.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaidentitygovernanceaccessreviewhistorydefinition
schema: 2.0.0
ms.subservice: entra-id-governance
---

# New-MgBetaIdentityGovernanceAccessReviewHistoryDefinition

## SYNOPSIS
Create a new accessReviewHistoryDefinition object.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgIdentityGovernanceAccessReviewHistoryDefinition](/powershell/module/Microsoft.Graph.Identity.Governance/New-MgIdentityGovernanceAccessReviewHistoryDefinition?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaIdentityGovernanceAccessReviewHistoryDefinition [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CreatedBy <IMicrosoftGraphUserIdentity>] [-CreatedDateTime <DateTime>]
 [-Decisions <String[]>] [-DisplayName <String>] [-DownloadUri <String>] [-FulfilledDateTime <DateTime>]
 [-Id <String>] [-Instances <IMicrosoftGraphAccessReviewHistoryInstance[]>]
 [-ReviewHistoryPeriodEndDateTime <DateTime>] [-ReviewHistoryPeriodStartDateTime <DateTime>]
 [-ScheduleSettings <IMicrosoftGraphAccessReviewHistoryScheduleSettings>]
 [-Scopes <IMicrosoftGraphAccessReviewScope[]>] [-Status <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaIdentityGovernanceAccessReviewHistoryDefinition
 -BodyParameter <IMicrosoftGraphAccessReviewHistoryDefinition> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new accessReviewHistoryDefinition object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | AccessReview.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | AccessReview.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	displayName = "Last quarter's group reviews April 2021"
	decisions = @(
	"approve"
"deny"
"dontKnow"
"notReviewed"
"notNotified"
)
reviewHistoryPeriodStartDateTime = [System.DateTime]::Parse("2021-01-01T00:00:00Z")
reviewHistoryPeriodEndDateTime = [System.DateTime]::Parse("2021-04-30T23:59:59Z")
scopes = @(
@{
"@odata.type" = "#microsoft.graph.accessReviewQueryScope"
queryType = "MicrosoftGraph"
query = "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')"
queryRoot = $null
}
@{
"@odata.type" = "#microsoft.graph.accessReviewQueryScope"
queryType = "MicrosoftGraph"
query = "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')"
queryRoot = $null
}
)
}

New-MgBetaIdentityGovernanceAccessReviewHistoryDefinition -BodyParameter $params

```
This example shows how to use the New-MgBetaIdentityGovernanceAccessReviewHistoryDefinition Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
accessReviewHistoryDefinition
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewHistoryDefinition
Parameter Sets: Create
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
userIdentity
To construct, see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserIdentity
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
Timestamp when the access review definition was created.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Decisions
Determines which review decisions will be included in the fetched review history data if specified.
Optional on create.
All decisions are included by default if no decisions are provided on create.
Possible values are: approve, deny, dontKnow, notReviewed, and notNotified.

```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Name for the access review history data collection.
Required.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DownloadUri


```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FulfilledDateTime


```yaml
Type: DateTime
Parameter Sets: CreateExpanded
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
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Instances
If the accessReviewHistoryDefinition is a recurring definition, instances represent each recurrence.
A definition that doesn't recur will have exactly one instance.
To construct, see NOTES section for INSTANCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewHistoryInstance[]
Parameter Sets: CreateExpanded
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

### -ReviewHistoryPeriodEndDateTime
A timestamp.
Reviews ending on or before this date will be included in the fetched history data.
Only required if scheduleSettings is not defined.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReviewHistoryPeriodStartDateTime
A timestamp.
Reviews starting on or before this date will be included in the fetched history data.
Only required if scheduleSettings isn't defined.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScheduleSettings
accessReviewHistoryScheduleSettings
To construct, see NOTES section for SCHEDULESETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewHistoryScheduleSettings
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Scopes
Used to scope what reviews are included in the fetched history data.
Fetches reviews whose scope matches with this provided scope.
Required.

```yaml
Type: IMicrosoftGraphAccessReviewScope[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
accessReviewHistoryStatus

```yaml
Type: String
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAccessReviewHistoryDefinition
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAccessReviewHistoryDefinition
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphAccessReviewHistoryDefinition>`: accessReviewHistoryDefinition
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CreatedBy <IMicrosoftGraphUserIdentity>]`: userIdentity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
    - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[IPAddress <String>]`: Indicates the client IP address associated with the user performing the activity (audit log only).
    - `[UserPrincipalName <String>]`: The userPrincipalName attribute of the user.
  - `[CreatedDateTime <DateTime?>]`: Timestamp when the access review definition was created.
  - `[Decisions <String- `[]`>]`: Determines which review decisions will be included in the fetched review history data if specified.
Optional on create.
All decisions are included by default if no decisions are provided on create.
Possible values are: approve, deny, dontKnow, notReviewed, and notNotified.
  - `[DisplayName <String>]`: Name for the access review history data collection.
Required.
  - `[DownloadUri <String>]`: 
  - `[FulfilledDateTime <DateTime?>]`: 
  - `[Instances <IMicrosoftGraphAccessReviewHistoryInstance- `[]`>]`: If the accessReviewHistoryDefinition is a recurring definition, instances represent each recurrence.
A definition that doesn't recur will have exactly one instance.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DownloadUri <String>]`: Uri that can be used to retrieve review history data.
This URI will be active for 24 hours after being generated.
Required.
    - `[ExpirationDateTime <DateTime?>]`: Timestamp when this instance and associated data expires and the history is deleted.
Required.
    - `[FulfilledDateTime <DateTime?>]`: Timestamp when all of the available data for this instance was collected.
This will be set after this instance's status is set to done.
Required.
    - `[ReviewHistoryPeriodEndDateTime <DateTime?>]`: The date and time for which reviews ended before this date are included in the fetched history data.
    - `[ReviewHistoryPeriodStartDateTime <DateTime?>]`: The date and time for which reviews started on or after this date are included in the fetched history data.
    - `[RunDateTime <DateTime?>]`: The date and time when the instance's history data is scheduled to be generated.
    - `[Status <String>]`: accessReviewHistoryStatus
  - `[ReviewHistoryPeriodEndDateTime <DateTime?>]`: A timestamp.
Reviews ending on or before this date will be included in the fetched history data.
Only required if scheduleSettings is not defined.
  - `[ReviewHistoryPeriodStartDateTime <DateTime?>]`: A timestamp.
Reviews starting on or before this date will be included in the fetched history data.
Only required if scheduleSettings isn't defined.
  - `[ScheduleSettings <IMicrosoftGraphAccessReviewHistoryScheduleSettings>]`: accessReviewHistoryScheduleSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
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
    - `[ReportRange <String>]`: A duration string in ISO 8601 duration format specifying the lookback period of the generated review history data.
For example, if a history definition is scheduled to run on the first of every month, the reportRange is P1M.
In this case, on the first of every month, access review history data is collected containing only the previous month's review data.
Note: Only years, months, and days ISO 8601 properties are supported.
Required.
  - `[Scopes <IMicrosoftGraphAccessReviewScope- `[]`>]`: Used to scope what reviews are included in the fetched history data.
Fetches reviews whose scope matches with this provided scope.
Required.
  - `[Status <String>]`: accessReviewHistoryStatus

CREATEDBY `<IMicrosoftGraphUserIdentity>`: userIdentity
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
  - `[Id <String>]`: The identifier of the identity.
This property is read-only.
  - `[IPAddress <String>]`: Indicates the client IP address associated with the user performing the activity (audit log only).
  - `[UserPrincipalName <String>]`: The userPrincipalName attribute of the user.

INSTANCES `<IMicrosoftGraphAccessReviewHistoryInstance- `[]`>`: If the accessReviewHistoryDefinition is a recurring definition, instances represent each recurrence.
A definition that doesn't recur will have exactly one instance.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DownloadUri <String>]`: Uri that can be used to retrieve review history data.
This URI will be active for 24 hours after being generated.
Required.
  - `[ExpirationDateTime <DateTime?>]`: Timestamp when this instance and associated data expires and the history is deleted.
Required.
  - `[FulfilledDateTime <DateTime?>]`: Timestamp when all of the available data for this instance was collected.
This will be set after this instance's status is set to done.
Required.
  - `[ReviewHistoryPeriodEndDateTime <DateTime?>]`: The date and time for which reviews ended before this date are included in the fetched history data.
  - `[ReviewHistoryPeriodStartDateTime <DateTime?>]`: The date and time for which reviews started on or after this date are included in the fetched history data.
  - `[RunDateTime <DateTime?>]`: The date and time when the instance's history data is scheduled to be generated.
  - `[Status <String>]`: accessReviewHistoryStatus

SCHEDULESETTINGS `<IMicrosoftGraphAccessReviewHistoryScheduleSettings>`: accessReviewHistoryScheduleSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
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
  - `[ReportRange <String>]`: A duration string in ISO 8601 duration format specifying the lookback period of the generated review history data.
For example, if a history definition is scheduled to run on the first of every month, the reportRange is P1M.
In this case, on the first of every month, access review history data is collected containing only the previous month's review data.
Note: Only years, months, and days ISO 8601 properties are supported.
Required.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaidentitygovernanceaccessreviewhistorydefinition](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaidentitygovernanceaccessreviewhistorydefinition)

[https://learn.microsoft.com/graph/api/accessreviewset-post-historydefinitions?view=graph-rest-beta](https://learn.microsoft.com/graph/api/accessreviewset-post-historydefinitions?view=graph-rest-beta)























