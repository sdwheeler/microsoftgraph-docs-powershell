---
external help file: Microsoft.Graph.Beta.Bookings-help.xml
Module Name: Microsoft.Graph.Beta.Bookings
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/update-mgbetavirtualeventwebinarsessionbyjoinweburl
schema: 2.0.0
---

# Update-MgBetaVirtualEventWebinarSessionByJoinWebUrl

## SYNOPSIS
Update the navigation property sessions in solutions

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaVirtualEventWebinarSessionByJoinWebUrl -JoinWebUrl <String> -VirtualEventWebinarId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-AllowAttendeeToEnableCamera]
 [-AllowAttendeeToEnableMic] [-AllowBreakoutRooms] [-AllowCopyingAndSharingMeetingContent]
 [-AllowLiveShare <String>] [-AllowMeetingChat <String>] [-AllowParticipantsToChangeName]
 [-AllowPowerPointSharing] [-AllowRecording] [-AllowTeamworkReactions] [-AllowTranscription] [-AllowWhiteboard]
 [-AllowedLobbyAdmitters <String>] [-AllowedPresenters <String>] [-AnonymizeIdentityForRoles <String[]>]
 [-AttendanceReports <IMicrosoftGraphMeetingAttendanceReport[]>]
 [-AudioConferencing <IMicrosoftGraphAudioConferencing>] [-ChatInfo <IMicrosoftGraphChatInfo>]
 [-ChatRestrictions <IMicrosoftGraphChatRestrictions>] [-EndDateTime <IMicrosoftGraphDateTimeZone>]
 [-Id <String>] [-IsEndToEndEncryptionEnabled] [-IsEntryExitAnnounced]
 [-JoinInformation <IMicrosoftGraphItemBody>] [-JoinMeetingIdSettings <IMicrosoftGraphJoinMeetingIdSettings>]
 [-JoinWebUrl1 <String>] [-LobbyBypassSettings <IMicrosoftGraphLobbyBypassSettings>]
 [-Presenters <IMicrosoftGraphVirtualEventPresenter[]>] [-RecordAutomatically]
 [-Registrations <IMicrosoftGraphVirtualEventRegistration[]>] [-ShareMeetingChatHistoryDefault <String>]
 [-StartDateTime <IMicrosoftGraphDateTimeZone>] [-Subject <String>] [-VideoOnDemandWebUrl <String>]
 [-VideoTeleconferenceId <String>] [-WatermarkProtection <IMicrosoftGraphWatermarkProtectionValues>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaVirtualEventWebinarSessionByJoinWebUrl [-JoinWebUrl <String>] -InputObject <IBookingsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-AllowAttendeeToEnableCamera]
 [-AllowAttendeeToEnableMic] [-AllowBreakoutRooms] [-AllowCopyingAndSharingMeetingContent]
 [-AllowLiveShare <String>] [-AllowMeetingChat <String>] [-AllowParticipantsToChangeName]
 [-AllowPowerPointSharing] [-AllowRecording] [-AllowTeamworkReactions] [-AllowTranscription] [-AllowWhiteboard]
 [-AllowedLobbyAdmitters <String>] [-AllowedPresenters <String>] [-AnonymizeIdentityForRoles <String[]>]
 [-AttendanceReports <IMicrosoftGraphMeetingAttendanceReport[]>]
 [-AudioConferencing <IMicrosoftGraphAudioConferencing>] [-ChatInfo <IMicrosoftGraphChatInfo>]
 [-ChatRestrictions <IMicrosoftGraphChatRestrictions>] [-EndDateTime <IMicrosoftGraphDateTimeZone>]
 [-Id <String>] [-IsEndToEndEncryptionEnabled] [-IsEntryExitAnnounced]
 [-JoinInformation <IMicrosoftGraphItemBody>] [-JoinMeetingIdSettings <IMicrosoftGraphJoinMeetingIdSettings>]
 [-LobbyBypassSettings <IMicrosoftGraphLobbyBypassSettings>]
 [-Presenters <IMicrosoftGraphVirtualEventPresenter[]>] [-RecordAutomatically]
 [-Registrations <IMicrosoftGraphVirtualEventRegistration[]>] [-ShareMeetingChatHistoryDefault <String>]
 [-StartDateTime <IMicrosoftGraphDateTimeZone>] [-Subject <String>] [-VideoOnDemandWebUrl <String>]
 [-VideoTeleconferenceId <String>] [-WatermarkProtection <IMicrosoftGraphWatermarkProtectionValues>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaVirtualEventWebinarSessionByJoinWebUrl -JoinWebUrl <String> -VirtualEventWebinarId <String>
 -BodyParameter <IMicrosoftGraphVirtualEventSession> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaVirtualEventWebinarSessionByJoinWebUrl -InputObject <IBookingsIdentity>
 -BodyParameter <IMicrosoftGraphVirtualEventSession> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property sessions in solutions

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

### -AllowAttendeeToEnableCamera
Indicates whether attendees can turn on their camera.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowAttendeeToEnableMic
Indicates whether attendees can turn on their microphone.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowBreakoutRooms
Indicates whether breakout rooms are enabled for the meeting.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowCopyingAndSharingMeetingContent
Indicates whether copying and sharing meeting content is enabled for the meeting.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowedLobbyAdmitters
allowedLobbyAdmitterRoles

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

### -AllowedPresenters
onlineMeetingPresenters

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

### -AllowLiveShare
meetingLiveShareOptions

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

### -AllowMeetingChat
meetingChatMode

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

### -AllowParticipantsToChangeName
Specifies if participants are allowed to rename themselves in an instance of the meeting.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowPowerPointSharing
Indicates whether PowerPoint live is enabled for the meeting.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowRecording
Indicates whether recording is enabled for the meeting.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowTeamworkReactions
Indicates if Teams reactions are enabled for the meeting.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowTranscription
Indicates whether transcription is enabled for the meeting.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowWhiteboard
Indicates whether whiteboard is enabled for the meeting.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AnonymizeIdentityForRoles
Specifies whose identity is anonymized in the meeting.
Possible values are: attendee.
The attendee value can't be removed through a PATCH operation once added.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AttendanceReports
The attendance reports of an online meeting.
Read-only.
To construct, see NOTES section for ATTENDANCEREPORTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMeetingAttendanceReport[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AudioConferencing
audioConferencing
To construct, see NOTES section for AUDIOCONFERENCING properties and create a hash table.

```yaml
Type: IMicrosoftGraphAudioConferencing
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
virtualEventSession
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphVirtualEventSession
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChatInfo
chatInfo
To construct, see NOTES section for CHATINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphChatInfo
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ChatRestrictions
chatRestrictions
To construct, see NOTES section for CHATRESTRICTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphChatRestrictions
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -EndDateTime
dateTimeTimeZone
To construct, see NOTES section for ENDDATETIME properties and create a hash table.

```yaml
Type: IMicrosoftGraphDateTimeZone
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
Type: IBookingsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsEndToEndEncryptionEnabled
Indicates whether end-to-end encryption (E2EE) is enabled for the online meeting.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsEntryExitAnnounced
Indicates whether to announce when callers join or leave.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -JoinInformation
itemBody
To construct, see NOTES section for JOININFORMATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphItemBody
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JoinMeetingIdSettings
joinMeetingIdSettings
To construct, see NOTES section for JOINMEETINGIDSETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphJoinMeetingIdSettings
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JoinWebUrl
Alternate key of virtualEventSession

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

```yaml
Type: String
Parameter Sets: UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JoinWebUrl1
The join URL of the online meeting.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LobbyBypassSettings
lobbyBypassSettings
To construct, see NOTES section for LOBBYBYPASSSETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphLobbyBypassSettings
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Presenters

To construct, see NOTES section for PRESENTERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphVirtualEventPresenter[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RecordAutomatically
Indicates whether to record the meeting automatically.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Registrations

To construct, see NOTES section for REGISTRATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphVirtualEventRegistration[]
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

### -ShareMeetingChatHistoryDefault
meetingChatHistoryDefaultMode

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

### -StartDateTime
dateTimeTimeZone
To construct, see NOTES section for STARTDATETIME properties and create a hash table.

```yaml
Type: IMicrosoftGraphDateTimeZone
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subject
The subject of the online meeting.

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

### -VideoOnDemandWebUrl


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

### -VideoTeleconferenceId
The video teleconferencing ID.
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

### -VirtualEventWebinarId
The unique identifier of virtualEventWebinar

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

### -WatermarkProtection
watermarkProtectionValues
To construct, see NOTES section for WATERMARKPROTECTION properties and create a hash table.

```yaml
Type: IMicrosoftGraphWatermarkProtectionValues
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IBookingsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphVirtualEventSession
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphVirtualEventSession
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ATTENDANCEREPORTS `<IMicrosoftGraphMeetingAttendanceReport- `[]`>`: The attendance reports of an online meeting.
Read-only.
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

AUDIOCONFERENCING `<IMicrosoftGraphAudioConferencing>`: audioConferencing
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ConferenceId <String>]`: The conference id of the online meeting.
  - `[DialinUrl <String>]`: A URL to the externally-accessible web page that contains dial-in information.
  - `[TollFreeNumber <String>]`: The toll-free number that connects to the Audio Conference Provider.
  - `[TollFreeNumbers <String- `[]`>]`: List of toll-free numbers that are displayed in the meeting invite.
  - `[TollNumber <String>]`: The toll number that connects to the Audio Conference Provider.
  - `[TollNumbers <String- `[]`>]`: List of toll numbers that are displayed in the meeting invite.

BODYPARAMETER `<IMicrosoftGraphVirtualEventSession>`: virtualEventSession
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AllowAttendeeToEnableCamera <Boolean?>]`: Indicates whether attendees can turn on their camera.
  - `[AllowAttendeeToEnableMic <Boolean?>]`: Indicates whether attendees can turn on their microphone.
  - `[AllowBreakoutRooms <Boolean?>]`: Indicates whether breakout rooms are enabled for the meeting.
  - `[AllowCopyingAndSharingMeetingContent <Boolean?>]`: Indicates whether copying and sharing meeting content is enabled for the meeting.
  - `[AllowLiveShare <String>]`: meetingLiveShareOptions
  - `[AllowMeetingChat <String>]`: meetingChatMode
  - `[AllowParticipantsToChangeName <Boolean?>]`: Specifies if participants are allowed to rename themselves in an instance of the meeting.
  - `[AllowPowerPointSharing <Boolean?>]`: Indicates whether PowerPoint live is enabled for the meeting.
  - `[AllowRecording <Boolean?>]`: Indicates whether recording is enabled for the meeting.
  - `[AllowTeamworkReactions <Boolean?>]`: Indicates if Teams reactions are enabled for the meeting.
  - `[AllowTranscription <Boolean?>]`: Indicates whether transcription is enabled for the meeting.
  - `[AllowWhiteboard <Boolean?>]`: Indicates whether whiteboard is enabled for the meeting.
  - `[AllowedLobbyAdmitters <String>]`: allowedLobbyAdmitterRoles
  - `[AllowedPresenters <String>]`: onlineMeetingPresenters
  - `[AnonymizeIdentityForRoles <String- `[]`>]`: Specifies whose identity is anonymized in the meeting.
Possible values are: attendee.
The attendee value can't be removed through a PATCH operation once added.
  - `[AttendanceReports <IMicrosoftGraphMeetingAttendanceReport- `[]`>]`: The attendance reports of an online meeting.
Read-only.
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
  - `[AudioConferencing <IMicrosoftGraphAudioConferencing>]`: audioConferencing
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ConferenceId <String>]`: The conference id of the online meeting.
    - `[DialinUrl <String>]`: A URL to the externally-accessible web page that contains dial-in information.
    - `[TollFreeNumber <String>]`: The toll-free number that connects to the Audio Conference Provider.
    - `[TollFreeNumbers <String- `[]`>]`: List of toll-free numbers that are displayed in the meeting invite.
    - `[TollNumber <String>]`: The toll number that connects to the Audio Conference Provider.
    - `[TollNumbers <String- `[]`>]`: List of toll numbers that are displayed in the meeting invite.
  - `[ChatInfo <IMicrosoftGraphChatInfo>]`: chatInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[MessageId <String>]`: The unique identifier for a message in a Microsoft Teams channel.
    - `[ReplyChainMessageId <String>]`: The ID of the reply message.
    - `[ThreadId <String>]`: The unique identifier for a thread in Microsoft Teams.
  - `[ChatRestrictions <IMicrosoftGraphChatRestrictions>]`: chatRestrictions
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowTextOnly <Boolean?>]`: Indicates whether only text is allowed in the meeting chat.
Optional.
  - `[IsEndToEndEncryptionEnabled <Boolean?>]`: Indicates whether end-to-end encryption (E2EE) is enabled for the online meeting.
  - `[IsEntryExitAnnounced <Boolean?>]`: Indicates whether to announce when callers join or leave.
  - `[JoinInformation <IMicrosoftGraphItemBody>]`: itemBody
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Content <String>]`: The content of the item.
    - `[ContentType <String>]`: bodyType
  - `[JoinMeetingIdSettings <IMicrosoftGraphJoinMeetingIdSettings>]`: joinMeetingIdSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsPasscodeRequired <Boolean?>]`: Indicates whether a passcode is required to join a meeting when using joinMeetingId.
Optional.
    - `[JoinMeetingId <String>]`: The meeting ID to be used to join a meeting.
Optional.
Read-only.
    - `[Passcode <String>]`: The passcode to join a meeting. 
Optional.
Read-only.
  - `[JoinWebUrl <String>]`: The join URL of the online meeting.
Read-only.
  - `[LobbyBypassSettings <IMicrosoftGraphLobbyBypassSettings>]`: lobbyBypassSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsDialInBypassEnabled <Boolean?>]`: Specifies whether or not to always let dial-in callers bypass the lobby.
Optional.
    - `[Scope <String>]`: lobbyBypassScope
  - `[RecordAutomatically <Boolean?>]`: Indicates whether to record the meeting automatically.
  - `[ShareMeetingChatHistoryDefault <String>]`: meetingChatHistoryDefaultMode
  - `[Subject <String>]`: The subject of the online meeting.
  - `[VideoTeleconferenceId <String>]`: The video teleconferencing ID.
Read-only.
  - `[WatermarkProtection <IMicrosoftGraphWatermarkProtectionValues>]`: watermarkProtectionValues
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsEnabledForContentSharing <Boolean?>]`: Indicates whether to apply a watermark to any shared content.
    - `[IsEnabledForVideo <Boolean?>]`: Indicates whether to apply a watermark to everyone's video feed.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[EndDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
    - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
  - `[Presenters <IMicrosoftGraphVirtualEventPresenter- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Email <String>]`: Email address of the presenter.
    - `[Identity <IMicrosoftGraphIdentity>]`: identity
    - `[PresenterDetails <IMicrosoftGraphVirtualEventPresenterDetails>]`: virtualEventPresenterDetails
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Bio <IMicrosoftGraphItemBody>]`: itemBody
      - `[Company <String>]`: The presenter's company name.
      - `[JobTitle <String>]`: The presenter's job title.
      - `[LinkedInProfileWebUrl <String>]`: The presenter's LinkedIn profile URL.
      - `[PersonalSiteWebUrl <String>]`: The presenter's personal website URL.
      - `[Photo <Byte- `[]`>]`: The content stream of the presenter's photo.
      - `[TwitterProfileWebUrl <String>]`: The presenter's Twitter profile URL.
    - `[Sessions <IMicrosoftGraphVirtualEventSession- `[]`>]`: 
  - `[Registrations <IMicrosoftGraphVirtualEventRegistration- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CancelationDateTime <DateTime?>]`: Date and time when the registrant cancels their registration for the virtual event.
Only appears when applicable.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[Email <String>]`: Email address of the registrant.
    - `[ExternalRegistrationInformation <IMicrosoftGraphVirtualEventExternalRegistrationInformation>]`: virtualEventExternalRegistrationInformation
    - `[FirstName <String>]`: First name of the registrant.
    - `[LastName <String>]`: Last name of the registrant.
    - `[PreferredLanguage <String>]`: The registrant's preferred language.
    - `[PreferredTimezone <String>]`: The registrant's time zone details.
    - `[RegistrantVideoOnDemandWebUrl <String>]`: 
    - `[RegistrationDateTime <DateTime?>]`: Date and time when the registrant registers for the virtual event.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[RegistrationQuestionAnswers <IMicrosoftGraphVirtualEventRegistrationQuestionAnswer- `[]`>]`: The registrant's answer to the registration questions.
      - `[BooleanValue <Boolean?>]`: Boolean answer to the virtualEventRegistrationCustomQuestion.
Only appears when answerInputType is boolean.
      - `[DisplayName <String>]`: Display name of the registration question.
      - `[MultiChoiceValues <String- `[]`>]`: A collection of text answers to the virtualEventRegistrationCustomQuestion.
Only appears when answerInputType is multiChoice.
      - `[QuestionId <String>]`: The identifier of either a virtualEventRegistrationCustomQuestion or a virtualEventRegistrationPredefinedQuestion.
      - `[Value <String>]`: Text answer to the virtualEventRegistrationCustomQuestion or the virtualEventRegistrationPredefinedQuestion.
Appears when answerInputType is text, multilineText or singleChoice.
    - `[Sessions <IMicrosoftGraphVirtualEventSession- `[]`>]`: 
    - `[Status <String>]`: virtualEventAttendeeRegistrationStatus
    - `[UserId <String>]`: The registrant's ID in Microsoft Entra ID.
Only appears when the registrant is registered in Microsoft Entra ID.
  - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
  - `[VideoOnDemandWebUrl <String>]`: 

CHATINFO `<IMicrosoftGraphChatInfo>`: chatInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[MessageId <String>]`: The unique identifier for a message in a Microsoft Teams channel.
  - `[ReplyChainMessageId <String>]`: The ID of the reply message.
  - `[ThreadId <String>]`: The unique identifier for a thread in Microsoft Teams.

CHATRESTRICTIONS `<IMicrosoftGraphChatRestrictions>`: chatRestrictions
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AllowTextOnly <Boolean?>]`: Indicates whether only text is allowed in the meeting chat.
Optional.

ENDDATETIME `<IMicrosoftGraphDateTimeZone>`: dateTimeTimeZone
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
  - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.

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

JOININFORMATION `<IMicrosoftGraphItemBody>`: itemBody
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Content <String>]`: The content of the item.
  - `[ContentType <String>]`: bodyType

JOINMEETINGIDSETTINGS `<IMicrosoftGraphJoinMeetingIdSettings>`: joinMeetingIdSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsPasscodeRequired <Boolean?>]`: Indicates whether a passcode is required to join a meeting when using joinMeetingId.
Optional.
  - `[JoinMeetingId <String>]`: The meeting ID to be used to join a meeting.
Optional.
Read-only.
  - `[Passcode <String>]`: The passcode to join a meeting. 
Optional.
Read-only.

LOBBYBYPASSSETTINGS `<IMicrosoftGraphLobbyBypassSettings>`: lobbyBypassSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsDialInBypassEnabled <Boolean?>]`: Specifies whether or not to always let dial-in callers bypass the lobby.
Optional.
  - `[Scope <String>]`: lobbyBypassScope

PRESENTERS `<IMicrosoftGraphVirtualEventPresenter- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Email <String>]`: Email address of the presenter.
  - `[Identity <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
    - `[Id <String>]`: The identifier of the identity.
This property is read-only.
  - `[PresenterDetails <IMicrosoftGraphVirtualEventPresenterDetails>]`: virtualEventPresenterDetails
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Bio <IMicrosoftGraphItemBody>]`: itemBody
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Content <String>]`: The content of the item.
      - `[ContentType <String>]`: bodyType
    - `[Company <String>]`: The presenter's company name.
    - `[JobTitle <String>]`: The presenter's job title.
    - `[LinkedInProfileWebUrl <String>]`: The presenter's LinkedIn profile URL.
    - `[PersonalSiteWebUrl <String>]`: The presenter's personal website URL.
    - `[Photo <Byte- `[]`>]`: The content stream of the presenter's photo.
    - `[TwitterProfileWebUrl <String>]`: The presenter's Twitter profile URL.
  - `[Sessions <IMicrosoftGraphVirtualEventSession- `[]`>]`: 
    - `[AllowAttendeeToEnableCamera <Boolean?>]`: Indicates whether attendees can turn on their camera.
    - `[AllowAttendeeToEnableMic <Boolean?>]`: Indicates whether attendees can turn on their microphone.
    - `[AllowBreakoutRooms <Boolean?>]`: Indicates whether breakout rooms are enabled for the meeting.
    - `[AllowCopyingAndSharingMeetingContent <Boolean?>]`: Indicates whether copying and sharing meeting content is enabled for the meeting.
    - `[AllowLiveShare <String>]`: meetingLiveShareOptions
    - `[AllowMeetingChat <String>]`: meetingChatMode
    - `[AllowParticipantsToChangeName <Boolean?>]`: Specifies if participants are allowed to rename themselves in an instance of the meeting.
    - `[AllowPowerPointSharing <Boolean?>]`: Indicates whether PowerPoint live is enabled for the meeting.
    - `[AllowRecording <Boolean?>]`: Indicates whether recording is enabled for the meeting.
    - `[AllowTeamworkReactions <Boolean?>]`: Indicates if Teams reactions are enabled for the meeting.
    - `[AllowTranscription <Boolean?>]`: Indicates whether transcription is enabled for the meeting.
    - `[AllowWhiteboard <Boolean?>]`: Indicates whether whiteboard is enabled for the meeting.
    - `[AllowedLobbyAdmitters <String>]`: allowedLobbyAdmitterRoles
    - `[AllowedPresenters <String>]`: onlineMeetingPresenters
    - `[AnonymizeIdentityForRoles <String- `[]`>]`: Specifies whose identity is anonymized in the meeting.
Possible values are: attendee.
The attendee value can't be removed through a PATCH operation once added.
    - `[AttendanceReports <IMicrosoftGraphMeetingAttendanceReport- `[]`>]`: The attendance reports of an online meeting.
Read-only.
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
    - `[AudioConferencing <IMicrosoftGraphAudioConferencing>]`: audioConferencing
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ConferenceId <String>]`: The conference id of the online meeting.
      - `[DialinUrl <String>]`: A URL to the externally-accessible web page that contains dial-in information.
      - `[TollFreeNumber <String>]`: The toll-free number that connects to the Audio Conference Provider.
      - `[TollFreeNumbers <String- `[]`>]`: List of toll-free numbers that are displayed in the meeting invite.
      - `[TollNumber <String>]`: The toll number that connects to the Audio Conference Provider.
      - `[TollNumbers <String- `[]`>]`: List of toll numbers that are displayed in the meeting invite.
    - `[ChatInfo <IMicrosoftGraphChatInfo>]`: chatInfo
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[MessageId <String>]`: The unique identifier for a message in a Microsoft Teams channel.
      - `[ReplyChainMessageId <String>]`: The ID of the reply message.
      - `[ThreadId <String>]`: The unique identifier for a thread in Microsoft Teams.
    - `[ChatRestrictions <IMicrosoftGraphChatRestrictions>]`: chatRestrictions
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AllowTextOnly <Boolean?>]`: Indicates whether only text is allowed in the meeting chat.
Optional.
    - `[IsEndToEndEncryptionEnabled <Boolean?>]`: Indicates whether end-to-end encryption (E2EE) is enabled for the online meeting.
    - `[IsEntryExitAnnounced <Boolean?>]`: Indicates whether to announce when callers join or leave.
    - `[JoinInformation <IMicrosoftGraphItemBody>]`: itemBody
    - `[JoinMeetingIdSettings <IMicrosoftGraphJoinMeetingIdSettings>]`: joinMeetingIdSettings
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsPasscodeRequired <Boolean?>]`: Indicates whether a passcode is required to join a meeting when using joinMeetingId.
Optional.
      - `[JoinMeetingId <String>]`: The meeting ID to be used to join a meeting.
Optional.
Read-only.
      - `[Passcode <String>]`: The passcode to join a meeting. 
Optional.
Read-only.
    - `[JoinWebUrl <String>]`: The join URL of the online meeting.
Read-only.
    - `[LobbyBypassSettings <IMicrosoftGraphLobbyBypassSettings>]`: lobbyBypassSettings
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsDialInBypassEnabled <Boolean?>]`: Specifies whether or not to always let dial-in callers bypass the lobby.
Optional.
      - `[Scope <String>]`: lobbyBypassScope
    - `[RecordAutomatically <Boolean?>]`: Indicates whether to record the meeting automatically.
    - `[ShareMeetingChatHistoryDefault <String>]`: meetingChatHistoryDefaultMode
    - `[Subject <String>]`: The subject of the online meeting.
    - `[VideoTeleconferenceId <String>]`: The video teleconferencing ID.
Read-only.
    - `[WatermarkProtection <IMicrosoftGraphWatermarkProtectionValues>]`: watermarkProtectionValues
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsEnabledForContentSharing <Boolean?>]`: Indicates whether to apply a watermark to any shared content.
      - `[IsEnabledForVideo <Boolean?>]`: Indicates whether to apply a watermark to everyone's video feed.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[EndDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
      - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
    - `[Presenters <IMicrosoftGraphVirtualEventPresenter- `[]`>]`: 
    - `[Registrations <IMicrosoftGraphVirtualEventRegistration- `[]`>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CancelationDateTime <DateTime?>]`: Date and time when the registrant cancels their registration for the virtual event.
Only appears when applicable.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[Email <String>]`: Email address of the registrant.
      - `[ExternalRegistrationInformation <IMicrosoftGraphVirtualEventExternalRegistrationInformation>]`: virtualEventExternalRegistrationInformation
      - `[FirstName <String>]`: First name of the registrant.
      - `[LastName <String>]`: Last name of the registrant.
      - `[PreferredLanguage <String>]`: The registrant's preferred language.
      - `[PreferredTimezone <String>]`: The registrant's time zone details.
      - `[RegistrantVideoOnDemandWebUrl <String>]`: 
      - `[RegistrationDateTime <DateTime?>]`: Date and time when the registrant registers for the virtual event.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[RegistrationQuestionAnswers <IMicrosoftGraphVirtualEventRegistrationQuestionAnswer- `[]`>]`: The registrant's answer to the registration questions.
        - `[BooleanValue <Boolean?>]`: Boolean answer to the virtualEventRegistrationCustomQuestion.
Only appears when answerInputType is boolean.
        - `[DisplayName <String>]`: Display name of the registration question.
        - `[MultiChoiceValues <String- `[]`>]`: A collection of text answers to the virtualEventRegistrationCustomQuestion.
Only appears when answerInputType is multiChoice.
        - `[QuestionId <String>]`: The identifier of either a virtualEventRegistrationCustomQuestion or a virtualEventRegistrationPredefinedQuestion.
        - `[Value <String>]`: Text answer to the virtualEventRegistrationCustomQuestion or the virtualEventRegistrationPredefinedQuestion.
Appears when answerInputType is text, multilineText or singleChoice.
      - `[Sessions <IMicrosoftGraphVirtualEventSession- `[]`>]`: 
      - `[Status <String>]`: virtualEventAttendeeRegistrationStatus
      - `[UserId <String>]`: The registrant's ID in Microsoft Entra ID.
Only appears when the registrant is registered in Microsoft Entra ID.
    - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[VideoOnDemandWebUrl <String>]`: 

REGISTRATIONS `<IMicrosoftGraphVirtualEventRegistration- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CancelationDateTime <DateTime?>]`: Date and time when the registrant cancels their registration for the virtual event.
Only appears when applicable.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[Email <String>]`: Email address of the registrant.
  - `[ExternalRegistrationInformation <IMicrosoftGraphVirtualEventExternalRegistrationInformation>]`: virtualEventExternalRegistrationInformation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Referrer <String>]`: A URL or string that represents the location from which the registrant registered.
Optional.
    - `[RegistrationId <String>]`: The identifier for a virtualEventExternalRegistrationInformation object.
Optional.
If set, the maximum supported length is 256 characters.
  - `[FirstName <String>]`: First name of the registrant.
  - `[LastName <String>]`: Last name of the registrant.
  - `[PreferredLanguage <String>]`: The registrant's preferred language.
  - `[PreferredTimezone <String>]`: The registrant's time zone details.
  - `[RegistrantVideoOnDemandWebUrl <String>]`: 
  - `[RegistrationDateTime <DateTime?>]`: Date and time when the registrant registers for the virtual event.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[RegistrationQuestionAnswers <IMicrosoftGraphVirtualEventRegistrationQuestionAnswer- `[]`>]`: The registrant's answer to the registration questions.
    - `[BooleanValue <Boolean?>]`: Boolean answer to the virtualEventRegistrationCustomQuestion.
Only appears when answerInputType is boolean.
    - `[DisplayName <String>]`: Display name of the registration question.
    - `[MultiChoiceValues <String- `[]`>]`: A collection of text answers to the virtualEventRegistrationCustomQuestion.
Only appears when answerInputType is multiChoice.
    - `[QuestionId <String>]`: The identifier of either a virtualEventRegistrationCustomQuestion or a virtualEventRegistrationPredefinedQuestion.
    - `[Value <String>]`: Text answer to the virtualEventRegistrationCustomQuestion or the virtualEventRegistrationPredefinedQuestion.
Appears when answerInputType is text, multilineText or singleChoice.
  - `[Sessions <IMicrosoftGraphVirtualEventSession- `[]`>]`: 
    - `[AllowAttendeeToEnableCamera <Boolean?>]`: Indicates whether attendees can turn on their camera.
    - `[AllowAttendeeToEnableMic <Boolean?>]`: Indicates whether attendees can turn on their microphone.
    - `[AllowBreakoutRooms <Boolean?>]`: Indicates whether breakout rooms are enabled for the meeting.
    - `[AllowCopyingAndSharingMeetingContent <Boolean?>]`: Indicates whether copying and sharing meeting content is enabled for the meeting.
    - `[AllowLiveShare <String>]`: meetingLiveShareOptions
    - `[AllowMeetingChat <String>]`: meetingChatMode
    - `[AllowParticipantsToChangeName <Boolean?>]`: Specifies if participants are allowed to rename themselves in an instance of the meeting.
    - `[AllowPowerPointSharing <Boolean?>]`: Indicates whether PowerPoint live is enabled for the meeting.
    - `[AllowRecording <Boolean?>]`: Indicates whether recording is enabled for the meeting.
    - `[AllowTeamworkReactions <Boolean?>]`: Indicates if Teams reactions are enabled for the meeting.
    - `[AllowTranscription <Boolean?>]`: Indicates whether transcription is enabled for the meeting.
    - `[AllowWhiteboard <Boolean?>]`: Indicates whether whiteboard is enabled for the meeting.
    - `[AllowedLobbyAdmitters <String>]`: allowedLobbyAdmitterRoles
    - `[AllowedPresenters <String>]`: onlineMeetingPresenters
    - `[AnonymizeIdentityForRoles <String- `[]`>]`: Specifies whose identity is anonymized in the meeting.
Possible values are: attendee.
The attendee value can't be removed through a PATCH operation once added.
    - `[AttendanceReports <IMicrosoftGraphMeetingAttendanceReport- `[]`>]`: The attendance reports of an online meeting.
Read-only.
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
    - `[AudioConferencing <IMicrosoftGraphAudioConferencing>]`: audioConferencing
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ConferenceId <String>]`: The conference id of the online meeting.
      - `[DialinUrl <String>]`: A URL to the externally-accessible web page that contains dial-in information.
      - `[TollFreeNumber <String>]`: The toll-free number that connects to the Audio Conference Provider.
      - `[TollFreeNumbers <String- `[]`>]`: List of toll-free numbers that are displayed in the meeting invite.
      - `[TollNumber <String>]`: The toll number that connects to the Audio Conference Provider.
      - `[TollNumbers <String- `[]`>]`: List of toll numbers that are displayed in the meeting invite.
    - `[ChatInfo <IMicrosoftGraphChatInfo>]`: chatInfo
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[MessageId <String>]`: The unique identifier for a message in a Microsoft Teams channel.
      - `[ReplyChainMessageId <String>]`: The ID of the reply message.
      - `[ThreadId <String>]`: The unique identifier for a thread in Microsoft Teams.
    - `[ChatRestrictions <IMicrosoftGraphChatRestrictions>]`: chatRestrictions
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AllowTextOnly <Boolean?>]`: Indicates whether only text is allowed in the meeting chat.
Optional.
    - `[IsEndToEndEncryptionEnabled <Boolean?>]`: Indicates whether end-to-end encryption (E2EE) is enabled for the online meeting.
    - `[IsEntryExitAnnounced <Boolean?>]`: Indicates whether to announce when callers join or leave.
    - `[JoinInformation <IMicrosoftGraphItemBody>]`: itemBody
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Content <String>]`: The content of the item.
      - `[ContentType <String>]`: bodyType
    - `[JoinMeetingIdSettings <IMicrosoftGraphJoinMeetingIdSettings>]`: joinMeetingIdSettings
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsPasscodeRequired <Boolean?>]`: Indicates whether a passcode is required to join a meeting when using joinMeetingId.
Optional.
      - `[JoinMeetingId <String>]`: The meeting ID to be used to join a meeting.
Optional.
Read-only.
      - `[Passcode <String>]`: The passcode to join a meeting. 
Optional.
Read-only.
    - `[JoinWebUrl <String>]`: The join URL of the online meeting.
Read-only.
    - `[LobbyBypassSettings <IMicrosoftGraphLobbyBypassSettings>]`: lobbyBypassSettings
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsDialInBypassEnabled <Boolean?>]`: Specifies whether or not to always let dial-in callers bypass the lobby.
Optional.
      - `[Scope <String>]`: lobbyBypassScope
    - `[RecordAutomatically <Boolean?>]`: Indicates whether to record the meeting automatically.
    - `[ShareMeetingChatHistoryDefault <String>]`: meetingChatHistoryDefaultMode
    - `[Subject <String>]`: The subject of the online meeting.
    - `[VideoTeleconferenceId <String>]`: The video teleconferencing ID.
Read-only.
    - `[WatermarkProtection <IMicrosoftGraphWatermarkProtectionValues>]`: watermarkProtectionValues
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsEnabledForContentSharing <Boolean?>]`: Indicates whether to apply a watermark to any shared content.
      - `[IsEnabledForVideo <Boolean?>]`: Indicates whether to apply a watermark to everyone's video feed.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[EndDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
      - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
    - `[Presenters <IMicrosoftGraphVirtualEventPresenter- `[]`>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Email <String>]`: Email address of the presenter.
      - `[Identity <IMicrosoftGraphIdentity>]`: identity
      - `[PresenterDetails <IMicrosoftGraphVirtualEventPresenterDetails>]`: virtualEventPresenterDetails
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Bio <IMicrosoftGraphItemBody>]`: itemBody
        - `[Company <String>]`: The presenter's company name.
        - `[JobTitle <String>]`: The presenter's job title.
        - `[LinkedInProfileWebUrl <String>]`: The presenter's LinkedIn profile URL.
        - `[PersonalSiteWebUrl <String>]`: The presenter's personal website URL.
        - `[Photo <Byte- `[]`>]`: The content stream of the presenter's photo.
        - `[TwitterProfileWebUrl <String>]`: The presenter's Twitter profile URL.
      - `[Sessions <IMicrosoftGraphVirtualEventSession- `[]`>]`: 
    - `[Registrations <IMicrosoftGraphVirtualEventRegistration- `[]`>]`: 
    - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[VideoOnDemandWebUrl <String>]`: 
  - `[Status <String>]`: virtualEventAttendeeRegistrationStatus
  - `[UserId <String>]`: The registrant's ID in Microsoft Entra ID.
Only appears when the registrant is registered in Microsoft Entra ID.

STARTDATETIME `<IMicrosoftGraphDateTimeZone>`: dateTimeTimeZone
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
  - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.

WATERMARKPROTECTION `<IMicrosoftGraphWatermarkProtectionValues>`: watermarkProtectionValues
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsEnabledForContentSharing <Boolean?>]`: Indicates whether to apply a watermark to any shared content.
  - `[IsEnabledForVideo <Boolean?>]`: Indicates whether to apply a watermark to everyone's video feed.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/update-mgbetavirtualeventwebinarsessionbyjoinweburl](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/update-mgbetavirtualeventwebinarsessionbyjoinweburl)
























