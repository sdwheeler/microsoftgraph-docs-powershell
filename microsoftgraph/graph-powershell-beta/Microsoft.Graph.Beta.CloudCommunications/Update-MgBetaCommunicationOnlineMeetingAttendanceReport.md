---
external help file: Microsoft.Graph.Beta.CloudCommunications-help.xml
Module Name: Microsoft.Graph.Beta.CloudCommunications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/update-mgbetacommunicationonlinemeetingattendancereport
schema: 2.0.0
---

# Update-MgBetaCommunicationOnlineMeetingAttendanceReport

## SYNOPSIS
Update the navigation property attendanceReports in communications

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgCommunicationOnlineMeetingAttendanceReport](/powershell/module/Microsoft.Graph.CloudCommunications/Update-MgCommunicationOnlineMeetingAttendanceReport?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded1 (Default)
```
Update-MgBetaCommunicationOnlineMeetingAttendanceReport -OnlineMeetingId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AttendanceRecords <IMicrosoftGraphAttendanceRecord[]>]
 [-ExternalEventInformation <IMicrosoftGraphVirtualEventExternalInformation[]>] [-Id <String>]
 [-MeetingEndDateTime <DateTime>] [-MeetingStartDateTime <DateTime>] [-TotalParticipantCount <Int32>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateExpanded
```
Update-MgBetaCommunicationOnlineMeetingAttendanceReport -MeetingAttendanceReportId <String>
 -OnlineMeetingId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AttendanceRecords <IMicrosoftGraphAttendanceRecord[]>]
 [-ExternalEventInformation <IMicrosoftGraphVirtualEventExternalInformation[]>] [-Id <String>]
 [-MeetingEndDateTime <DateTime>] [-MeetingStartDateTime <DateTime>] [-TotalParticipantCount <Int32>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaCommunicationOnlineMeetingAttendanceReport -MeetingAttendanceReportId <String>
 -OnlineMeetingId <String> -BodyParameter <IMicrosoftGraphMeetingAttendanceReport>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Update1
```
Update-MgBetaCommunicationOnlineMeetingAttendanceReport -OnlineMeetingId <String>
 -BodyParameter <IMicrosoftGraphMeetingAttendanceReport> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded1
```
Update-MgBetaCommunicationOnlineMeetingAttendanceReport -InputObject <ICloudCommunicationsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AttendanceRecords <IMicrosoftGraphAttendanceRecord[]>]
 [-ExternalEventInformation <IMicrosoftGraphVirtualEventExternalInformation[]>] [-Id <String>]
 [-MeetingEndDateTime <DateTime>] [-MeetingStartDateTime <DateTime>] [-TotalParticipantCount <Int32>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaCommunicationOnlineMeetingAttendanceReport -InputObject <ICloudCommunicationsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AttendanceRecords <IMicrosoftGraphAttendanceRecord[]>]
 [-ExternalEventInformation <IMicrosoftGraphVirtualEventExternalInformation[]>] [-Id <String>]
 [-MeetingEndDateTime <DateTime>] [-MeetingStartDateTime <DateTime>] [-TotalParticipantCount <Int32>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity1
```
Update-MgBetaCommunicationOnlineMeetingAttendanceReport -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IMicrosoftGraphMeetingAttendanceReport> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaCommunicationOnlineMeetingAttendanceReport -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IMicrosoftGraphMeetingAttendanceReport> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property attendanceReports in communications

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AttendanceRecords
List of attendance records of an attendance report.
Read-only.
To construct, see NOTES section for ATTENDANCERECORDS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAttendanceRecord[]
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
meetingAttendanceReport
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphMeetingAttendanceReport
Parameter Sets: Update, Update1, UpdateViaIdentity1, UpdateViaIdentity
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

### -ExternalEventInformation
The external information of a virtual event.
Returned only for event organizers or coorganizers.
Read-only.
To construct, see NOTES section for EXTERNALEVENTINFORMATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphVirtualEventExternalInformation[]
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
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
Type: ICloudCommunicationsIdentity
Parameter Sets: UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded, UpdateViaIdentity1, UpdateViaIdentity
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
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MeetingEndDateTime
UTC time when the meeting ended.
Read-only.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MeetingStartDateTime
UTC time when the meeting started.
Read-only.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OnlineMeetingId
The unique identifier of onlineMeeting

```yaml
Type: String
Parameter Sets: UpdateExpanded1, UpdateExpanded, Update, Update1
Aliases:

Required: True
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

### -TotalParticipantCount
Total number of participants.
Read-only.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
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

### Microsoft.Graph.Beta.PowerShell.Models.ICloudCommunicationsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMeetingAttendanceReport
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMeetingAttendanceReport
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ATTENDANCERECORDS `<IMicrosoftGraphAttendanceRecord- `[]`>`: List of attendance records of an attendance report.
Read-only.
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

BODYPARAMETER `<IMicrosoftGraphMeetingAttendanceReport>`: meetingAttendanceReport
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AttendanceRecords <IMicrosoftGraphAttendanceRecord- `[]`>]`: List of attendance records of an attendance report.
Read-only.
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
  - `[ExternalEventInformation <IMicrosoftGraphVirtualEventExternalInformation- `[]`>]`: The external information of a virtual event.
Returned only for event organizers or coorganizers.
Read-only.
    - `[ApplicationId <String>]`: Identifier of the application that hosts the externalEventId.
Read-only.
    - `[ExternalEventId <String>]`: The identifier for a virtualEventExternalInformation object that associates the virtual event with an event ID in an external application.
This association bundles all the information (both supported and not supported in virtualEvent) into one virtual event object.
Optional.
If set, the maximum supported length is 256 characters.
  - `[MeetingEndDateTime <DateTime?>]`: UTC time when the meeting ended.
Read-only.
  - `[MeetingStartDateTime <DateTime?>]`: UTC time when the meeting started.
Read-only.
  - `[TotalParticipantCount <Int32?>]`: Total number of participants.
Read-only.

EXTERNALEVENTINFORMATION `<IMicrosoftGraphVirtualEventExternalInformation- `[]`>`: The external information of a virtual event.
Returned only for event organizers or coorganizers.
Read-only.
  - `[ApplicationId <String>]`: Identifier of the application that hosts the externalEventId.
Read-only.
  - `[ExternalEventId <String>]`: The identifier for a virtualEventExternalInformation object that associates the virtual event with an event ID in an external application.
This association bundles all the information (both supported and not supported in virtualEvent) into one virtual event object.
Optional.
If set, the maximum supported length is 256 characters.

INPUTOBJECT `<ICloudCommunicationsIdentity>`: Identity Parameter
  - `[AttendanceRecordId <String>]`: The unique identifier of attendanceRecord
  - `[AudioRoutingGroupId <String>]`: The unique identifier of audioRoutingGroup
  - `[CallAiInsightId <String>]`: The unique identifier of callAiInsight
  - `[CallId <String>]`: The unique identifier of call
  - `[CallRecordId <String>]`: The unique identifier of callRecord
  - `[CallRecordingId <String>]`: The unique identifier of callRecording
  - `[CallTranscriptId <String>]`: The unique identifier of callTranscript
  - `[CommsOperationId <String>]`: The unique identifier of commsOperation
  - `[ContentSharingSessionId <String>]`: The unique identifier of contentSharingSession
  - `[FromDateTime <DateTime?>]`: Usage: fromDateTime={fromDateTime}
  - `[JoinWebUrl <String>]`: Alternate key of onlineMeeting
  - `[MeetingAttendanceReportId <String>]`: The unique identifier of meetingAttendanceReport
  - `[MeetingRegistrantBaseId <String>]`: The unique identifier of meetingRegistrantBase
  - `[MeetingRegistrationQuestionId <String>]`: The unique identifier of meetingRegistrationQuestion
  - `[OnlineMeetingId <String>]`: The unique identifier of onlineMeeting
  - `[ParticipantId <String>]`: The unique identifier of participant
  - `[PresenceId <String>]`: The unique identifier of presence
  - `[SessionId <String>]`: The unique identifier of session
  - `[ToDateTime <DateTime?>]`: Usage: toDateTime={toDateTime}
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/update-mgbetacommunicationonlinemeetingattendancereport](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/update-mgbetacommunicationonlinemeetingattendancereport)
























