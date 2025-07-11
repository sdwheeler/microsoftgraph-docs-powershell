---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/set-mguserpresenceuserpreferredpresence
schema: 2.0.0
ms.subservice: cloud-communications
---

# Set-MgUserPresenceUserPreferredPresence

## SYNOPSIS
Set the preferred availability and activity status for a user.
If the preferred presence of a user is set, the user's presence shows as the preferred status.
Preferred presence takes effect only when at least one presence session exists for the user.
Otherwise, the user's presence shows as Offline.
A presence session is created as a result of a successful setPresence operation, or if the user is signed in on a Microsoft Teams client.
For more details, see presence sessions and time-out and expiration.

> [!NOTE]
> To view the beta release of this cmdlet, view [Set-MgBetaUserPresenceUserPreferredPresence](/powershell/module/Microsoft.Graph.Beta.CloudCommunications/Set-MgBetaUserPresenceUserPreferredPresence?view=graph-powershell-beta)

## SYNTAX

### SetExpanded (Default)
```
Set-MgUserPresenceUserPreferredPresence -UserId <String> [-ResponseHeadersVariable <String>]
 [-Activity <String>] [-AdditionalProperties <Hashtable>] [-Availability <String>]
 [-ExpirationDuration <TimeSpan>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Set
```
Set-MgUserPresenceUserPreferredPresence -UserId <String>
 -BodyParameter <IPathsTrjrarUsersUserIdPresenceMicrosoftGraphSetuserpreferredpresencePostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentityExpanded
```
Set-MgUserPresenceUserPreferredPresence -InputObject <ICloudCommunicationsIdentity>
 [-ResponseHeadersVariable <String>] [-Activity <String>] [-AdditionalProperties <Hashtable>]
 [-Availability <String>] [-ExpirationDuration <TimeSpan>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentity
```
Set-MgUserPresenceUserPreferredPresence -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IPathsTrjrarUsersUserIdPresenceMicrosoftGraphSetuserpreferredpresencePostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Set the preferred availability and activity status for a user.
If the preferred presence of a user is set, the user's presence shows as the preferred status.
Preferred presence takes effect only when at least one presence session exists for the user.
Otherwise, the user's presence shows as Offline.
A presence session is created as a result of a successful setPresence operation, or if the user is signed in on a Microsoft Teams client.
For more details, see presence sessions and time-out and expiration.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Presence.ReadWrite,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Presence.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	availability = "DoNotDisturb"
	activity = "DoNotDisturb"
	expirationDuration = "PT8H"
}

Set-MgUserPresenceUserPreferredPresence -UserId $userId -BodyParameter $params

```
This example shows how to use the Set-MgUserPresenceUserPreferredPresence Cmdlet.


## PARAMETERS

### -Activity


```yaml
Type: String
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Availability


```yaml
Type: String
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter

To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPathsTrjrarUsersUserIdPresenceMicrosoftGraphSetuserpreferredpresencePostRequestbodyContentApplicationJsonSchema
Parameter Sets: Set, SetViaIdentity
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

### -ExpirationDuration


```yaml
Type: TimeSpan
Parameter Sets: SetExpanded, SetViaIdentityExpanded
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ICloudCommunicationsIdentity
Parameter Sets: SetViaIdentityExpanded, SetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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
Parameter Sets: SetExpanded, Set
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

### Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity
### Microsoft.Graph.PowerShell.Models.IPathsTrjrarUsersUserIdPresenceMicrosoftGraphSetuserpreferredpresencePostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsTrjrarUsersUserIdPresenceMicrosoftGraphSetuserpreferredpresencePostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Activity <String>]`:
  - `[Availability <String>]`:
  - `[ExpirationDuration <TimeSpan?>]`:

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/set-mguserpresenceuserpreferredpresence](https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/set-mguserpresenceuserpreferredpresence)

[https://learn.microsoft.com/graph/api/presence-setuserpreferredpresence?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/presence-setuserpreferredpresence?view=graph-rest-1.0)























