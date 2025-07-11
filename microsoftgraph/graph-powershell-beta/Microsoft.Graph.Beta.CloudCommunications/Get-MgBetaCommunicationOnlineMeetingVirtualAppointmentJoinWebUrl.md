---
external help file: Microsoft.Graph.Beta.CloudCommunications-help.xml
Module Name: Microsoft.Graph.Beta.CloudCommunications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/get-mgbetacommunicationonlinemeetingvirtualappointmentjoinweburl
schema: 2.0.0
ms.subservice: cloud-communications
---

# Get-MgBetaCommunicationOnlineMeetingVirtualAppointmentJoinWebUrl

## SYNOPSIS
Get a join web URL for a Teams Virtual Appointment.
This web URL includes enhanced business-to-customer experiences such as mobile browser join and virtual lobby rooms.
With Teams Premium, you can configure a custom lobby room experience for attendees by adding your company logo and access the Virtual Appointments usage report for organizational analytics.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgCommunicationOnlineMeetingVirtualAppointmentJoinWebUrl](/powershell/module/Microsoft.Graph.CloudCommunications/Get-MgCommunicationOnlineMeetingVirtualAppointmentJoinWebUrl?view=graph-powershell-1.0)

## SYNTAX

### Get (Default)
```
Get-MgBetaCommunicationOnlineMeetingVirtualAppointmentJoinWebUrl -OnlineMeetingId <String>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaCommunicationOnlineMeetingVirtualAppointmentJoinWebUrl -InputObject <ICloudCommunicationsIdentity>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Get a join web URL for a Teams Virtual Appointment.
This web URL includes enhanced business-to-customer experiences such as mobile browser join and virtual lobby rooms.
With Teams Premium, you can configure a custom lobby room experience for attendees by adding your company logo and access the Virtual Appointments usage report for organizational analytics.

## EXAMPLES

## PARAMETERS

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
Type: ICloudCommunicationsIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OnlineMeetingId
The unique identifier of onlineMeeting

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.ICloudCommunicationsIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.String
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/get-mgbetacommunicationonlinemeetingvirtualappointmentjoinweburl](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/get-mgbetacommunicationonlinemeetingvirtualappointmentjoinweburl)

[https://learn.microsoft.com/graph/api/virtualappointment-getvirtualappointmentjoinweburl?view=graph-rest-beta](https://learn.microsoft.com/graph/api/virtualappointment-getvirtualappointmentjoinweburl?view=graph-rest-beta)
























