---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/get-mguseronlinemeetingattendeereport
schema: 2.0.0
---

# Get-MgUserOnlineMeetingAttendeeReport

## SYNOPSIS
The content stream of the attendee report of a Microsoft Teams live event.
Read-only.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaUserOnlineMeetingAttendeeReport](/powershell/module/Microsoft.Graph.Beta.CloudCommunications/Get-MgBetaUserOnlineMeetingAttendeeReport?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgUserOnlineMeetingAttendeeReport -OnlineMeetingId <String> -UserId <String> -OutFile <String>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgUserOnlineMeetingAttendeeReport -InputObject <ICloudCommunicationsIdentity> -OutFile <String>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [<CommonParameters>]
```

## DESCRIPTION
The content stream of the attendee report of a Microsoft Teams live event.
Read-only.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | OnlineMeetingArtifact.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | OnlineMeetingArtifact.Read.All,  |

## EXAMPLES
### Example 1: Fetch attendee report of a Teams live event

```powershell

Import-Module Microsoft.Graph.CloudCommunications

# A UPN can also be used as -UserId.
Get-MgUserOnlineMeetingAttendeeReport -UserId $userId -OnlineMeetingId $onlineMeetingId

```
This example will fetch attendee report of a teams live event


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

### Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity
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
  - `[CallId <String>]`: The unique identifier of call
  - `[CallRecordId <String>]`: The unique identifier of callRecord
  - `[CallRecordingId <String>]`: The unique identifier of callRecording
  - `[CallTranscriptId <String>]`: The unique identifier of callTranscript
  - `[CommsOperationId <String>]`: The unique identifier of commsOperation
  - `[ContentSharingSessionId <String>]`: The unique identifier of contentSharingSession
  - `[MeetingAttendanceReportId <String>]`: The unique identifier of meetingAttendanceReport
  - `[OnlineMeetingId <String>]`: The unique identifier of onlineMeeting
  - `[ParticipantId <String>]`: The unique identifier of participant
  - `[PresenceId <String>]`: The unique identifier of presence
  - `[SessionId <String>]`: The unique identifier of session
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/get-mguseronlinemeetingattendeereport](https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/get-mguseronlinemeetingattendeereport)























