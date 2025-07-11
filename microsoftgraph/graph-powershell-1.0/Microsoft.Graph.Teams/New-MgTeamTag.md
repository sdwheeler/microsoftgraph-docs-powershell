---
external help file: Microsoft.Graph.Teams-help.xml
Module Name: Microsoft.Graph.Teams
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.teams/new-mgteamtag
schema: 2.0.0
ms.subservice: teams
---

# New-MgTeamTag

## SYNOPSIS
Create a standard tag for members in a team.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaTeamTag](/powershell/module/Microsoft.Graph.Beta.Teams/New-MgBetaTeamTag?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgTeamTag -TeamId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>] [-MemberCount <Int32>]
 [-Members <IMicrosoftGraphTeamworkTagMember[]>] [-TagType <String>] [-TeamId1 <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgTeamTag [-TeamId <String>] -InputObject <ITeamsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Description <String>] [-DisplayName <String>] [-Id <String>]
 [-MemberCount <Int32>] [-Members <IMicrosoftGraphTeamworkTagMember[]>] [-TagType <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgTeamTag -TeamId <String> -BodyParameter <IMicrosoftGraphTeamworkTag> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgTeamTag -InputObject <ITeamsIdentity> -BodyParameter <IMicrosoftGraphTeamworkTag>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a standard tag for members in a team.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | TeamworkTag.ReadWrite,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | TeamworkTag.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
	displayName = "Finance"
	members = @(
		@{
			userId = "92f6952f-61ca-4a94-8910-508a240bc167"
		}
		@{
			userId = "085d800c-b86b-4bfc-a857-9371ad1caf29"
		}
	)
}

New-MgTeamTag -TeamId $teamId -BodyParameter $params

```
This example shows how to use the New-MgTeamTag Cmdlet.


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

### -BodyParameter
teamworkTag
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamworkTag
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

### -Description
The description of the tag as it appears to the user in Microsoft Teams.
A teamworkTag can't have more than 200 teamworkTagMembers.

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

### -DisplayName
The name of the tag as it appears to the user in Microsoft Teams.

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ITeamsIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MemberCount
The number of users assigned to the tag.

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

### -Members
Users assigned to the tag.
To construct, see NOTES section for MEMBERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamworkTagMember[]
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

### -TagType
teamworkTagType

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

### -TeamId
The unique identifier of team

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

```yaml
Type: String
Parameter Sets: CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TeamId1
ID of the team in which the tag is defined.

```yaml
Type: String
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTeamworkTag
### Microsoft.Graph.PowerShell.Models.ITeamsIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTeamworkTag
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphTeamworkTag>`: teamworkTag
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Description <String>]`: The description of the tag as it appears to the user in Microsoft Teams.
A teamworkTag can't have more than 200 teamworkTagMembers.
  - `[DisplayName <String>]`: The name of the tag as it appears to the user in Microsoft Teams.
  - `[MemberCount <Int32?>]`: The number of users assigned to the tag.
  - `[Members <IMicrosoftGraphTeamworkTagMember- `[]`>]`: Users assigned to the tag.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: The member's display name.
    - `[TenantId <String>]`: The ID of the tenant that the tag member is a part of.
    - `[UserId <String>]`: The user ID of the member.
  - `[TagType <String>]`: teamworkTagType
  - `[TeamId <String>]`: ID of the team in which the tag is defined.

INPUTOBJECT `<ITeamsIdentity>`: Identity Parameter
  - `[AssociatedTeamInfoId <String>]`: The unique identifier of associatedTeamInfo
  - `[ChannelId <String>]`: The unique identifier of channel
  - `[ChatId <String>]`: The unique identifier of chat
  - `[ChatMessageHostedContentId <String>]`: The unique identifier of chatMessageHostedContent
  - `[ChatMessageId <String>]`: The unique identifier of chatMessage
  - `[ChatMessageId1 <String>]`: The unique identifier of chatMessage
  - `[ConversationMemberId <String>]`: The unique identifier of conversationMember
  - `[DayNoteId <String>]`: The unique identifier of dayNote
  - `[DeletedChatId <String>]`: The unique identifier of deletedChat
  - `[DeletedTeamId <String>]`: The unique identifier of deletedTeam
  - `[GroupId <String>]`: The unique identifier of group
  - `[OfferShiftRequestId <String>]`: The unique identifier of offerShiftRequest
  - `[OpenShiftChangeRequestId <String>]`: The unique identifier of openShiftChangeRequest
  - `[OpenShiftId <String>]`: The unique identifier of openShift
  - `[PinnedChatMessageInfoId <String>]`: The unique identifier of pinnedChatMessageInfo
  - `[ResourceSpecificPermissionGrantId <String>]`: The unique identifier of resourceSpecificPermissionGrant
  - `[SchedulingGroupId <String>]`: The unique identifier of schedulingGroup
  - `[SharedWithChannelTeamInfoId <String>]`: The unique identifier of sharedWithChannelTeamInfo
  - `[ShiftId <String>]`: The unique identifier of shift
  - `[SwapShiftsChangeRequestId <String>]`: The unique identifier of swapShiftsChangeRequest
  - `[TeamId <String>]`: The unique identifier of team
  - `[TeamsAppDefinitionId <String>]`: The unique identifier of teamsAppDefinition
  - `[TeamsAppId <String>]`: The unique identifier of teamsApp
  - `[TeamsAppInstallationId <String>]`: The unique identifier of teamsAppInstallation
  - `[TeamsAsyncOperationId <String>]`: The unique identifier of teamsAsyncOperation
  - `[TeamsTabId <String>]`: The unique identifier of teamsTab
  - `[TeamworkTagId <String>]`: The unique identifier of teamworkTag
  - `[TeamworkTagMemberId <String>]`: The unique identifier of teamworkTagMember
  - `[TimeCardId <String>]`: The unique identifier of timeCard
  - `[TimeOffId <String>]`: The unique identifier of timeOff
  - `[TimeOffReasonId <String>]`: The unique identifier of timeOffReason
  - `[TimeOffRequestId <String>]`: The unique identifier of timeOffRequest
  - `[UserId <String>]`: The unique identifier of user
  - `[UserScopeTeamsAppInstallationId <String>]`: The unique identifier of userScopeTeamsAppInstallation
  - `[WorkforceIntegrationId <String>]`: The unique identifier of workforceIntegration

MEMBERS `<IMicrosoftGraphTeamworkTagMember- `[]`>`: Users assigned to the tag.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The member's display name.
  - `[TenantId <String>]`: The ID of the tenant that the tag member is a part of.
  - `[UserId <String>]`: The user ID of the member.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.teams/new-mgteamtag](https://learn.microsoft.com/powershell/module/microsoft.graph.teams/new-mgteamtag)

[https://learn.microsoft.com/graph/api/teamworktag-post?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/teamworktag-post?view=graph-rest-1.0)























