---
external help file: Microsoft.Graph.Beta.CloudCommunications-help.xml
Module Name: Microsoft.Graph.Beta.CloudCommunications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/update-mgbetauseronlinemeetingaiinsight
schema: 2.0.0
---

# Update-MgBetaUserOnlineMeetingAiInsight

## SYNOPSIS
Update the navigation property aiInsights in users

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaUserOnlineMeetingAiInsight -CallAiInsightId <String> -OnlineMeetingId <String> -UserId <String>
 [-ResponseHeadersVariable <String>] [-ActionItems <IMicrosoftGraphActionItem[]>]
 [-AdditionalProperties <Hashtable>] [-CallId <String>] [-ContentCorrelationId <String>]
 [-CreatedDateTime <DateTime>] [-EndDateTime <DateTime>] [-Id <String>]
 [-MeetingNotes <IMicrosoftGraphMeetingNote[]>] [-Viewpoint <IMicrosoftGraphCallAiInsightViewPoint>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaUserOnlineMeetingAiInsight -CallAiInsightId <String> -OnlineMeetingId <String> -UserId <String>
 -BodyParameter <IMicrosoftGraphCallAiInsight> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaUserOnlineMeetingAiInsight -InputObject <ICloudCommunicationsIdentity>
 [-ResponseHeadersVariable <String>] [-ActionItems <IMicrosoftGraphActionItem[]>]
 [-AdditionalProperties <Hashtable>] [-CallId <String>] [-ContentCorrelationId <String>]
 [-CreatedDateTime <DateTime>] [-EndDateTime <DateTime>] [-Id <String>]
 [-MeetingNotes <IMicrosoftGraphMeetingNote[]>] [-Viewpoint <IMicrosoftGraphCallAiInsightViewPoint>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaUserOnlineMeetingAiInsight -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IMicrosoftGraphCallAiInsight> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property aiInsights in users

## EXAMPLES

## PARAMETERS

### -ActionItems

To construct, see NOTES section for ACTIONITEMS properties and create a hash table.

```yaml
Type: IMicrosoftGraphActionItem[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
callAiInsight
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphCallAiInsight
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CallAiInsightId
The unique identifier of callAiInsight

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

### -CallId


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

### -ContentCorrelationId


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

### -CreatedDateTime


```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndDateTime


```yaml
Type: DateTime
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
Type: ICloudCommunicationsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MeetingNotes

To construct, see NOTES section for MEETINGNOTES properties and create a hash table.

```yaml
Type: IMicrosoftGraphMeetingNote[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, Update
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

### -UserId
The unique identifier of user

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

### -Viewpoint
callAiInsightViewPoint
To construct, see NOTES section for VIEWPOINT properties and create a hash table.

```yaml
Type: IMicrosoftGraphCallAiInsightViewPoint
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

### Microsoft.Graph.Beta.PowerShell.Models.ICloudCommunicationsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphCallAiInsight
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphCallAiInsight
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ACTIONITEMS `<IMicrosoftGraphActionItem- `[]`>`: .
  - `[OwnerDisplayName <String>]`: 
  - `[Text <String>]`: 
  - `[Title <String>]`: 

BODYPARAMETER `<IMicrosoftGraphCallAiInsight>`: callAiInsight
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActionItems <IMicrosoftGraphActionItem- `[]`>]`: 
    - `[OwnerDisplayName <String>]`: 
    - `[Text <String>]`: 
    - `[Title <String>]`: 
  - `[CallId <String>]`: 
  - `[ContentCorrelationId <String>]`: 
  - `[CreatedDateTime <DateTime?>]`: 
  - `[EndDateTime <DateTime?>]`: 
  - `[MeetingNotes <IMicrosoftGraphMeetingNote- `[]`>]`: 
    - `[Subpoints <IMicrosoftGraphMeetingNoteSubpoint- `[]`>]`: 
      - `[Text <String>]`: 
      - `[Title <String>]`: 
    - `[Text <String>]`: 
    - `[Title <String>]`: 
  - `[Viewpoint <IMicrosoftGraphCallAiInsightViewPoint>]`: callAiInsightViewPoint
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[MentionEvents <IMicrosoftGraphMentionEvent- `[]`>]`: 
      - `[EventDateTime <DateTime?>]`: 
      - `[Speaker <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Application <IMicrosoftGraphIdentity>]`: identity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
          - `[Id <String>]`: The identifier of the identity.
This property is read-only.
        - `[Device <IMicrosoftGraphIdentity>]`: identity
        - `[User <IMicrosoftGraphIdentity>]`: identity
      - `[TranscriptUtterance <String>]`: 

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

MEETINGNOTES `<IMicrosoftGraphMeetingNote- `[]`>`: .
  - `[Subpoints <IMicrosoftGraphMeetingNoteSubpoint- `[]`>]`: 
    - `[Text <String>]`: 
    - `[Title <String>]`: 
  - `[Text <String>]`: 
  - `[Title <String>]`: 

VIEWPOINT `<IMicrosoftGraphCallAiInsightViewPoint>`: callAiInsightViewPoint
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[MentionEvents <IMicrosoftGraphMentionEvent- `[]`>]`: 
    - `[EventDateTime <DateTime?>]`: 
    - `[Speaker <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
        - `[Id <String>]`: The identifier of the identity.
This property is read-only.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[TranscriptUtterance <String>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/update-mgbetauseronlinemeetingaiinsight](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.cloudcommunications/update-mgbetauseronlinemeetingaiinsight)
























