---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/invoke-mgredirectcommunicationcall
schema: 2.0.0
ms.subservice: cloud-communications
---

# Invoke-MgRedirectCommunicationCall

## SYNOPSIS
Redirect an incoming call that hasn't been answered or rejected yet.
The terms 'redirecting' and 'forwarding' a call are used interchangeably.
The bot is expected to redirect the call before the call times out.
The current timeout value is 15 seconds.

> [!NOTE]
> To view the beta release of this cmdlet, view [Invoke-MgBetaRedirectCommunicationCall](/powershell/module/Microsoft.Graph.Beta.CloudCommunications/Invoke-MgBetaRedirectCommunicationCall?view=graph-powershell-beta)

## SYNTAX

### RedirectExpanded (Default)
```
Invoke-MgRedirectCommunicationCall -CallId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CallbackUri <String>]
 [-Targets <IMicrosoftGraphInvitationParticipantInfo[]>] [-Timeout <Int32>] [-Headers <IDictionary>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Redirect
```
Invoke-MgRedirectCommunicationCall -CallId <String>
 -BodyParameter <IPaths183Gi8UCommunicationsCallsCallIdMicrosoftGraphRedirectPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RedirectViaIdentityExpanded
```
Invoke-MgRedirectCommunicationCall -InputObject <ICloudCommunicationsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-CallbackUri <String>]
 [-Targets <IMicrosoftGraphInvitationParticipantInfo[]>] [-Timeout <Int32>] [-Headers <IDictionary>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RedirectViaIdentity
```
Invoke-MgRedirectCommunicationCall -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IPaths183Gi8UCommunicationsCallsCallIdMicrosoftGraphRedirectPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Redirect an incoming call that hasn't been answered or rejected yet.
The terms 'redirecting' and 'forwarding' a call are used interchangeably.
The bot is expected to redirect the call before the call times out.
The current timeout value is 15 seconds.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	targets = @(
		@{
			"@odata.type" = "#microsoft.graph.invitationParticipantInfo"
			identity = @{
				"@odata.type" = "#microsoft.graph.identitySet"
				phone = @{
					"@odata.type" = "#microsoft.graph.identity"
					id = "+12345678901"
				}
			}
		}
	)
	callbackUri = "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}

Invoke-MgRedirectCommunicationCall -CallId $callId -BodyParameter $params

```
This example shows how to use the Invoke-MgRedirectCommunicationCall Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: RedirectExpanded, RedirectViaIdentityExpanded
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
Type: IPaths183Gi8UCommunicationsCallsCallIdMicrosoftGraphRedirectPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Redirect, RedirectViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CallbackUri


```yaml
Type: String
Parameter Sets: RedirectExpanded, RedirectViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CallId
The unique identifier of call

```yaml
Type: String
Parameter Sets: RedirectExpanded, Redirect
Aliases:

Required: True
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
Parameter Sets: RedirectViaIdentityExpanded, RedirectViaIdentity
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

### -Targets

To construct, see NOTES section for TARGETS properties and create a hash table.

```yaml
Type: IMicrosoftGraphInvitationParticipantInfo[]
Parameter Sets: RedirectExpanded, RedirectViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Timeout


```yaml
Type: Int32
Parameter Sets: RedirectExpanded, RedirectViaIdentityExpanded
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

### Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths183Gi8UCommunicationsCallsCallIdMicrosoftGraphRedirectPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths183Gi8UCommunicationsCallsCallIdMicrosoftGraphRedirectPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CallbackUri <String>]`:
  - `[Targets <IMicrosoftGraphInvitationParticipantInfo- `[]`>]`:
    - `[Hidden <Boolean?>]`: Optional.
Whether to hide the participant from the roster.
    - `[Identity <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[ParticipantId <String>]`: Optional.
The ID of the target participant.
    - `[RemoveFromDefaultAudioRoutingGroup <Boolean?>]`: Optional.
Whether to remove them from the main mixer.
    - `[ReplacesCallId <String>]`: Optional.
The call which the target identity is currently a part of.
For peer-to-peer case, the call will be dropped once the participant is added successfully.
  - `[Timeout <Int32?>]`:

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

TARGETS `<IMicrosoftGraphInvitationParticipantInfo- `[]`>`: .
  - `[Hidden <Boolean?>]`: Optional.
Whether to hide the participant from the roster.
  - `[Identity <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[ParticipantId <String>]`: Optional.
The ID of the target participant.
  - `[RemoveFromDefaultAudioRoutingGroup <Boolean?>]`: Optional.
Whether to remove them from the main mixer.
  - `[ReplacesCallId <String>]`: Optional.
The call which the target identity is currently a part of.
For peer-to-peer case, the call will be dropped once the participant is added successfully.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/invoke-mgredirectcommunicationcall](https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/invoke-mgredirectcommunicationcall)

[https://learn.microsoft.com/graph/api/call-redirect?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/call-redirect?view=graph-rest-1.0)























