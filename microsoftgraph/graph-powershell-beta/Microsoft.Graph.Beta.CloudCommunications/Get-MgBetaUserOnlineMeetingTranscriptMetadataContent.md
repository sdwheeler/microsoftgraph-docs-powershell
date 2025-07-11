---
external help file: Microsoft.Graph.Beta.CloudCommunications-help.xml
Module Name: Microsoft.Graph.Beta.CloudCommunications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/get-mgbetauseronlinemeetingtranscriptmetadatacontent
schema: 2.0.0
ms.subservice: teams
---

# Get-MgBetaUserOnlineMeetingTranscriptMetadataContent

## SYNOPSIS
Retrieve a callTranscript object associated with a scheduled onlineMeeting.
This API supports the retrieval of call transcripts from private chat meetings and channel meetings.
Retrieving the transcript returns the metadata of the single transcript associated with the online meeting.
Retrieving the content of the transcript returns the stream of text associated with the transcript.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgUserOnlineMeetingTranscriptMetadataContent](/powershell/module/Microsoft.Graph.CloudCommunications/Get-MgUserOnlineMeetingTranscriptMetadataContent?view=graph-powershell-1.0)

## SYNTAX

### Get (Default)
```
Get-MgBetaUserOnlineMeetingTranscriptMetadataContent -CallTranscriptId <String> -OnlineMeetingId <String>
 -UserId <String> -OutFile <String> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaUserOnlineMeetingTranscriptMetadataContent -InputObject <ICloudCommunicationsIdentity>
 -OutFile <String> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [<CommonParameters>]
```

## DESCRIPTION
Retrieve a callTranscript object associated with a scheduled onlineMeeting.
This API supports the retrieval of call transcripts from private chat meetings and channel meetings.
Retrieving the transcript returns the metadata of the single transcript associated with the online meeting.
Retrieving the content of the transcript returns the stream of text associated with the transcript.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | OnlineMeetingTranscript.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | OnlineMeetingTranscript.Read.All, OnlineMeetingTranscript.Read.Chat,  |

## EXAMPLES
### Example 1: Get a callTranscript metadataContent

```powershell

Import-Module Microsoft.Graph.Beta.CloudCommunications

Get-MgBetaUserOnlineMeetingTranscriptMetadataContent -UserId $userId -OnlineMeetingId $onlineMeetingId -CallTranscriptId $callTranscriptId

```
This example will get a calltranscript metadatacontent


## PARAMETERS

### -CallTranscriptId
The unique identifier of callTranscript

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

### -OutFile
Path to write output file to

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
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

### Microsoft.Graph.Beta.PowerShell.Models.ICloudCommunicationsIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
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

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/get-mgbetauseronlinemeetingtranscriptmetadatacontent](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/get-mgbetauseronlinemeetingtranscriptmetadatacontent)

[https://learn.microsoft.com/graph/api/calltranscript-get?view=graph-rest-beta](https://learn.microsoft.com/graph/api/calltranscript-get?view=graph-rest-beta)























