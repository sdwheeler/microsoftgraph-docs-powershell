---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/move-mgcommunicationcall
schema: 2.0.0
ms.subservice: cloud-communications
---

# Move-MgCommunicationCall

## SYNOPSIS
Transfer an active peer-to-peer call or group call.
A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.
This is opposed to transfering the call directly.

> [!NOTE]
> To view the beta release of this cmdlet, view [Move-MgBetaCommunicationCall](/powershell/module/Microsoft.Graph.Beta.CloudCommunications/Move-MgBetaCommunicationCall?view=graph-powershell-beta)

## SYNTAX

### TransferExpanded (Default)
```
Move-MgCommunicationCall -CallId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-TransferTarget <IMicrosoftGraphInvitationParticipantInfo>]
 [-Transferee <IMicrosoftGraphParticipantInfo>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Transfer
```
Move-MgCommunicationCall -CallId <String>
 -BodyParameter <IPaths4Zbm7LCommunicationsCallsCallIdMicrosoftGraphTransferPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### TransferViaIdentityExpanded
```
Move-MgCommunicationCall -InputObject <ICloudCommunicationsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-TransferTarget <IMicrosoftGraphInvitationParticipantInfo>]
 [-Transferee <IMicrosoftGraphParticipantInfo>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### TransferViaIdentity
```
Move-MgCommunicationCall -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IPaths4Zbm7LCommunicationsCallsCallIdMicrosoftGraphTransferPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Transfer an active peer-to-peer call or group call.
A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.
This is opposed to transfering the call directly.

## EXAMPLES
### Example 1: Call transfer from a peer-to-peer call

```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	transferTarget = @{
		endpointType = "default"
		identity = @{
			user = @{
				id = "550fae72-d251-43ec-868c-373732c2704f"
				displayName = "Heidi Steen"
			}
		}
	}
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```
This example will call transfer from a peer-to-peer call

### Example 2: Consultative transfer from a peer-to-peer call

```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	transferTarget = @{
		"@odata.type" = "#microsoft.graph.invitationParticipantInfo"
		endpointType = "default"
		identity = @{
			"@odata.type" = "#microsoft.graph.identitySet"
			user = @{
				"@odata.type" = "#microsoft.graph.identity"
				id = "550fae72-d251-43ec-868c-373732c2704f"
				displayName = "Heidi Steen"
			}
		}
		replacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d"
	}
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```
This example will consultative transfer from a peer-to-peer call

### Example 3: Call transfer from a peer-to-peer call to PSTN number

```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	transferTarget = @{
		endpointType = "default"
		identity = @{
			phone = @{
				"@odata.type" = "#microsoft.graph.identity"
				id = "+12345678901"
			}
		}
		languageId = "languageId-value"
		region = "region-value"
	}
	clientContext = "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```
This example will call transfer from a peer-to-peer call to pstn number

### Example 4: Consultative transfer from a peer-to-peer call to PSTN number

```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	transferTarget = @{
		"@odata.type" = "#microsoft.graph.invitationParticipantInfo"
		endpointType = "default"
		identity = @{
			"@odata.type" = "#microsoft.graph.identitySet"
			phone = @{
				"@odata.type" = "#microsoft.graph.identity"
				id = "+12345678901"
			}
		}
		languageId = "en-us"
		region = "amer"
		replacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d"
	}
	clientContext = "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```
This example will consultative transfer from a peer-to-peer call to pstn number

### Example 5: Call transfer from a group call

```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	transferTarget = @{
		endpointType = "default"
		identity = @{
			user = @{
				id = "550fae72-d251-43ec-868c-373732c2704f"
				displayName = "Heidi Steen"
			}
		}
	}
	transferee = @{
		identity = @{
			user = @{
				id = "751f6800-3180-414d-bd94-333364659951"
				tenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47"
			}
		}
		participantId = "909c6581-5130-43e9-88f3-fcb3582cde37"
	}
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```
This example will call transfer from a group call


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: TransferExpanded, TransferViaIdentityExpanded
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
Type: IPaths4Zbm7LCommunicationsCallsCallIdMicrosoftGraphTransferPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Transfer, TransferViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CallId
The unique identifier of call

```yaml
Type: String
Parameter Sets: TransferExpanded, Transfer
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
Parameter Sets: TransferViaIdentityExpanded, TransferViaIdentity
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

### -Transferee
participantInfo
To construct, see NOTES section for TRANSFEREE properties and create a hash table.

```yaml
Type: IMicrosoftGraphParticipantInfo
Parameter Sets: TransferExpanded, TransferViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TransferTarget
invitationParticipantInfo
To construct, see NOTES section for TRANSFERTARGET properties and create a hash table.

```yaml
Type: IMicrosoftGraphInvitationParticipantInfo
Parameter Sets: TransferExpanded, TransferViaIdentityExpanded
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

### Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths4Zbm7LCommunicationsCallsCallIdMicrosoftGraphTransferPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths4Zbm7LCommunicationsCallsCallIdMicrosoftGraphTransferPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[TransferTarget <IMicrosoftGraphInvitationParticipantInfo>]`: invitationParticipantInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
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
  - `[Transferee <IMicrosoftGraphParticipantInfo>]`: participantInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CountryCode <String>]`: The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.
Read-only.
    - `[EndpointType <String>]`: endpointType
    - `[Identity <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LanguageId <String>]`: The language culture string.
Read-only.
    - `[ParticipantId <String>]`: The participant ID of the participant.
Read-only.
    - `[Region <String>]`: The home region of the participant.
This can be a country, a continent, or a larger geographic region.
This doesn't change based on the participant's current physical location.
Read-only.

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

TRANSFEREE `<IMicrosoftGraphParticipantInfo>`: participantInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CountryCode <String>]`: The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.
Read-only.
  - `[EndpointType <String>]`: endpointType
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
  - `[LanguageId <String>]`: The language culture string.
Read-only.
  - `[ParticipantId <String>]`: The participant ID of the participant.
Read-only.
  - `[Region <String>]`: The home region of the participant.
This can be a country, a continent, or a larger geographic region.
This doesn't change based on the participant's current physical location.
Read-only.

TRANSFERTARGET `<IMicrosoftGraphInvitationParticipantInfo>`: invitationParticipantInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
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

[https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/move-mgcommunicationcall](https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/move-mgcommunicationcall)

[https://learn.microsoft.com/graph/api/call-transfer?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/call-transfer?view=graph-rest-1.0)























