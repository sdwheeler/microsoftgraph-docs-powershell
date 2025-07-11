---
external help file: Microsoft.Graph.Beta.Bookings-help.xml
Module Name: Microsoft.Graph.Beta.Bookings
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/new-mgbetavirtualeventsessionattendancereportattendancerecord
schema: 2.0.0
---

# New-MgBetaVirtualEventSessionAttendanceReportAttendanceRecord

## SYNOPSIS
Create new navigation property to attendanceRecords for solutions

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgVirtualEventSessionAttendanceReportAttendanceRecord](/powershell/module/Microsoft.Graph.Bookings/New-MgVirtualEventSessionAttendanceReportAttendanceRecord?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaVirtualEventSessionAttendanceReportAttendanceRecord -MeetingAttendanceReportId <String>
 -VirtualEventId <String> -VirtualEventSessionId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AttendanceIntervals <IMicrosoftGraphAttendanceInterval[]>]
 [-EmailAddress <String>]
 [-ExternalRegistrationInformation <IMicrosoftGraphVirtualEventExternalRegistrationInformation>] [-Id <String>]
 [-Identity <IMicrosoftGraphIdentity>] [-RegistrantId <String>] [-RegistrationId <String>] [-Role <String>]
 [-TotalAttendanceInSeconds <Int32>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaVirtualEventSessionAttendanceReportAttendanceRecord -MeetingAttendanceReportId <String>
 -VirtualEventId <String> -VirtualEventSessionId <String> -BodyParameter <IMicrosoftGraphAttendanceRecord>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaVirtualEventSessionAttendanceReportAttendanceRecord -InputObject <IBookingsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AttendanceIntervals <IMicrosoftGraphAttendanceInterval[]>] [-EmailAddress <String>]
 [-ExternalRegistrationInformation <IMicrosoftGraphVirtualEventExternalRegistrationInformation>] [-Id <String>]
 [-Identity <IMicrosoftGraphIdentity>] [-RegistrantId <String>] [-RegistrationId <String>] [-Role <String>]
 [-TotalAttendanceInSeconds <Int32>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaVirtualEventSessionAttendanceReportAttendanceRecord -InputObject <IBookingsIdentity>
 -BodyParameter <IMicrosoftGraphAttendanceRecord> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to attendanceRecords for solutions

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

### -AttendanceIntervals
List of time periods between joining and leaving a meeting.
To construct, see NOTES section for ATTENDANCEINTERVALS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAttendanceInterval[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
attendanceRecord
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAttendanceRecord
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

### -EmailAddress
Email address of the user associated with this attendance record.

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

### -ExternalRegistrationInformation
virtualEventExternalRegistrationInformation
To construct, see NOTES section for EXTERNALREGISTRATIONINFORMATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphVirtualEventExternalRegistrationInformation
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
identity
To construct, see NOTES section for IDENTITY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentity
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
Type: IBookingsIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MeetingAttendanceReportId
The unique identifier of meetingAttendanceReport

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

### -RegistrantId
Unique identifier of a meetingRegistrant.
Presents when the participant has registered for the meeting.
(deprecated)

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

### -RegistrationId
Unique identifier of a virtualEventRegistration.
Presents for all participant who has registered for the virtualEventWebinar.

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

### -Role
Role of the attendee.
Possible values are: None, Attendee, Presenter, and Organizer.

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

### -TotalAttendanceInSeconds
Total duration of the attendances in seconds.

```yaml
Type: Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -VirtualEventId
The unique identifier of virtualEvent

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

### -VirtualEventSessionId
The unique identifier of virtualEventSession

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

### Microsoft.Graph.Beta.PowerShell.Models.IBookingsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAttendanceRecord
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAttendanceRecord
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ATTENDANCEINTERVALS `<IMicrosoftGraphAttendanceInterval- `[]`>`: List of time periods between joining and leaving a meeting.
  - `[DurationInSeconds <Int32?>]`: Duration of the meeting interval in seconds; that is, the difference between joinDateTime and leaveDateTime.
  - `[JoinDateTime <DateTime?>]`: The time the attendee joined in UTC.
  - `[LeaveDateTime <DateTime?>]`: The time the attendee left in UTC.

BODYPARAMETER `<IMicrosoftGraphAttendanceRecord>`: attendanceRecord
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AttendanceIntervals <IMicrosoftGraphAttendanceInterval- `[]`>]`: List of time periods between joining and leaving a meeting.
    - `[DurationInSeconds <Int32?>]`: Duration of the meeting interval in seconds; that is, the difference between joinDateTime and leaveDateTime.
    - `[JoinDateTime <DateTime?>]`: The time the attendee joined in UTC.
    - `[LeaveDateTime <DateTime?>]`: The time the attendee left in UTC.
  - `[EmailAddress <String>]`: Email address of the user associated with this attendance record.
  - `[ExternalRegistrationInformation <IMicrosoftGraphVirtualEventExternalRegistrationInformation>]`: virtualEventExternalRegistrationInformation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Referrer <String>]`: A URL or string that represents the location from which the registrant registered.
Optional.
    - `[RegistrationId <String>]`: The identifier for a virtualEventExternalRegistrationInformation object.
Optional.
If set, the maximum supported length is 256 characters.
  - `[Identity <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
    - `[Id <String>]`: The identifier of the identity.
This property is read-only.
  - `[RegistrantId <String>]`: Unique identifier of a meetingRegistrant.
Presents when the participant has registered for the meeting.
(deprecated)
  - `[RegistrationId <String>]`: Unique identifier of a virtualEventRegistration.
Presents for all participant who has registered for the virtualEventWebinar.
  - `[Role <String>]`: Role of the attendee.
Possible values are: None, Attendee, Presenter, and Organizer.
  - `[TotalAttendanceInSeconds <Int32?>]`: Total duration of the attendances in seconds.

EXTERNALREGISTRATIONINFORMATION `<IMicrosoftGraphVirtualEventExternalRegistrationInformation>`: virtualEventExternalRegistrationInformation
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Referrer <String>]`: A URL or string that represents the location from which the registrant registered.
Optional.
  - `[RegistrationId <String>]`: The identifier for a virtualEventExternalRegistrationInformation object.
Optional.
If set, the maximum supported length is 256 characters.

IDENTITY `<IMicrosoftGraphIdentity>`: identity
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
  - `[Id <String>]`: The identifier of the identity.
This property is read-only.

INPUTOBJECT `<IBookingsIdentity>`: Identity Parameter
  - `[AttendanceRecordId <String>]`: The unique identifier of attendanceRecord
  - `[BookingAppointmentId <String>]`: The unique identifier of bookingAppointment
  - `[BookingBusinessId <String>]`: The unique identifier of bookingBusiness
  - `[BookingCurrencyId <String>]`: The unique identifier of bookingCurrency
  - `[BookingCustomQuestionId <String>]`: The unique identifier of bookingCustomQuestion
  - `[BookingCustomerId <String>]`: The unique identifier of bookingCustomer
  - `[BookingServiceId <String>]`: The unique identifier of bookingService
  - `[BookingStaffMemberId <String>]`: The unique identifier of bookingStaffMember
  - `[Email <String>]`: Alternate key of virtualEventRegistration
  - `[JoinWebUrl <String>]`: Alternate key of virtualEventSession
  - `[MeetingAttendanceReportId <String>]`: The unique identifier of meetingAttendanceReport
  - `[Role <String>]`: Usage: role='{role}'
  - `[UserId <String>]`: Alternate key of virtualEventRegistration
  - `[VirtualEventId <String>]`: The unique identifier of virtualEvent
  - `[VirtualEventPresenterId <String>]`: The unique identifier of virtualEventPresenter
  - `[VirtualEventRegistrationId <String>]`: The unique identifier of virtualEventRegistration
  - `[VirtualEventRegistrationQuestionBaseId <String>]`: The unique identifier of virtualEventRegistrationQuestionBase
  - `[VirtualEventSessionId <String>]`: The unique identifier of virtualEventSession
  - `[VirtualEventTownhallId <String>]`: The unique identifier of virtualEventTownhall
  - `[VirtualEventWebinarId <String>]`: The unique identifier of virtualEventWebinar

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/new-mgbetavirtualeventsessionattendancereportattendancerecord](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/new-mgbetavirtualeventsessionattendancereportattendancerecord)
























