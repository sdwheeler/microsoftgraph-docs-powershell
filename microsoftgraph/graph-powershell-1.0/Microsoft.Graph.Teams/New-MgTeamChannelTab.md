---
external help file: Microsoft.Graph.Teams-help.xml
Module Name: Microsoft.Graph.Teams
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.teams/new-mgteamchanneltab
schema: 2.0.0
ms.subservice: teams
---

# New-MgTeamChannelTab

## SYNOPSIS
Add (pin) a tab to the specified channel within a team.
The app must be preinstalled in the team and have the configurableTabs property defined in the app manifest.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaTeamChannelTab](/powershell/module/Microsoft.Graph.Beta.Teams/New-MgBetaTeamChannelTab?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgTeamChannelTab -ChannelId <String> -TeamId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Configuration <IMicrosoftGraphTeamsTabConfiguration>]
 [-DisplayName <String>] [-Id <String>] [-TeamsApp <IMicrosoftGraphTeamsApp>] [-WebUrl <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgTeamChannelTab -ChannelId <String> -TeamId <String> -BodyParameter <IMicrosoftGraphTeamsTab>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgTeamChannelTab -InputObject <ITeamsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Configuration <IMicrosoftGraphTeamsTabConfiguration>]
 [-DisplayName <String>] [-Id <String>] [-TeamsApp <IMicrosoftGraphTeamsApp>] [-WebUrl <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgTeamChannelTab -InputObject <ITeamsIdentity> -BodyParameter <IMicrosoftGraphTeamsTab>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Add (pin) a tab to the specified channel within a team.
The app must be preinstalled in the team and have the configurableTabs property defined in the app manifest.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | TeamsTab.Create, TeamsTab.ReadWriteSelfForTeam, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | TeamsTab.Create.Group, TeamsTab.ReadWriteSelfForTeam.All, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, TeamsTab.Create, Group.ReadWrite.All, Directory.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
	displayName = "My Contoso Tab"
	"teamsApp@odata.bind" = "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8"
	configuration = @{
		entityId = "2DCA2E6C7A10415CAF6B8AB6661B3154"
		contentUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView"
		websiteUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154"
		removeUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
	}
}

New-MgTeamChannelTab -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```
This example shows how to use the New-MgTeamChannelTab Cmdlet.


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
teamsTab
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsTab
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChannelId
The unique identifier of channel

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

### -Configuration
teamsTabConfiguration
To construct, see NOTES section for CONFIGURATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsTabConfiguration
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### -DisplayName
Name of the tab.

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

### -TeamsApp
teamsApp
To construct, see NOTES section for TEAMSAPP properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsApp
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebUrl
Deep link URL of the tab instance.
Read only.

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTeamsTab
### Microsoft.Graph.PowerShell.Models.ITeamsIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTeamsTab
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphTeamsTab>`: teamsTab
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Configuration <IMicrosoftGraphTeamsTabConfiguration>]`: teamsTabConfiguration
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ContentUrl <String>]`: Url used for rendering tab contents in Teams.
Required.
    - `[EntityId <String>]`: Identifier for the entity hosted by the tab provider.
    - `[RemoveUrl <String>]`: Url called by Teams client when a Tab is removed using the Teams Client.
    - `[WebsiteUrl <String>]`: Url for showing tab contents outside of Teams.
  - `[DisplayName <String>]`: Name of the tab.
  - `[TeamsApp <IMicrosoftGraphTeamsApp>]`: teamsApp
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppDefinitions <IMicrosoftGraphTeamsAppDefinition- `[]`>]`: The details for each version of the app.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Authorization <IMicrosoftGraphTeamsAppAuthorization>]`: teamsAppAuthorization
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[ClientAppId <String>]`: The registration ID of the Microsoft Entra app ID associated with the teamsApp.
        - `[RequiredPermissionSet <IMicrosoftGraphTeamsAppPermissionSet>]`: teamsAppPermissionSet
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[ResourceSpecificPermissions <IMicrosoftGraphTeamsAppResourceSpecificPermission- `[]`>]`: A collection of resource-specific permissions.
            - `[PermissionType <String>]`: teamsAppResourceSpecificPermissionType
            - `[PermissionValue <String>]`: The name of the resource-specific permission.
      - `[Bot <IMicrosoftGraphTeamworkBot>]`: teamworkBot
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Application <IMicrosoftGraphIdentity>]`: identity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
          - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
        - `[Device <IMicrosoftGraphIdentity>]`: identity
        - `[User <IMicrosoftGraphIdentity>]`: identity
      - `[Description <String>]`: Verbose description of the application.
      - `[DisplayName <String>]`: The name of the app provided by the app developer.
      - `[LastModifiedDateTime <DateTime?>]`:
      - `[PublishingState <String>]`: teamsAppPublishingState
      - `[ShortDescription <String>]`: Short description of the application.
      - `[TeamsAppId <String>]`: The ID from the Teams app manifest.
      - `[Version <String>]`: The version number of the application.
    - `[DisplayName <String>]`: The name of the catalog app provided by the app developer in the Microsoft Teams zip app package.
    - `[DistributionMethod <String>]`: teamsAppDistributionMethod
    - `[ExternalId <String>]`: The ID of the catalog provided by the app developer in the Microsoft Teams zip app package.
  - `[WebUrl <String>]`: Deep link URL of the tab instance.
Read only.

CONFIGURATION `<IMicrosoftGraphTeamsTabConfiguration>`: teamsTabConfiguration
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ContentUrl <String>]`: Url used for rendering tab contents in Teams.
Required.
  - `[EntityId <String>]`: Identifier for the entity hosted by the tab provider.
  - `[RemoveUrl <String>]`: Url called by Teams client when a Tab is removed using the Teams Client.
  - `[WebsiteUrl <String>]`: Url for showing tab contents outside of Teams.

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

TEAMSAPP `<IMicrosoftGraphTeamsApp>`: teamsApp
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AppDefinitions <IMicrosoftGraphTeamsAppDefinition- `[]`>]`: The details for each version of the app.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Authorization <IMicrosoftGraphTeamsAppAuthorization>]`: teamsAppAuthorization
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ClientAppId <String>]`: The registration ID of the Microsoft Entra app ID associated with the teamsApp.
      - `[RequiredPermissionSet <IMicrosoftGraphTeamsAppPermissionSet>]`: teamsAppPermissionSet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[ResourceSpecificPermissions <IMicrosoftGraphTeamsAppResourceSpecificPermission- `[]`>]`: A collection of resource-specific permissions.
          - `[PermissionType <String>]`: teamsAppResourceSpecificPermissionType
          - `[PermissionValue <String>]`: The name of the resource-specific permission.
    - `[Bot <IMicrosoftGraphTeamworkBot>]`: teamworkBot
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[Description <String>]`: Verbose description of the application.
    - `[DisplayName <String>]`: The name of the app provided by the app developer.
    - `[LastModifiedDateTime <DateTime?>]`:
    - `[PublishingState <String>]`: teamsAppPublishingState
    - `[ShortDescription <String>]`: Short description of the application.
    - `[TeamsAppId <String>]`: The ID from the Teams app manifest.
    - `[Version <String>]`: The version number of the application.
  - `[DisplayName <String>]`: The name of the catalog app provided by the app developer in the Microsoft Teams zip app package.
  - `[DistributionMethod <String>]`: teamsAppDistributionMethod
  - `[ExternalId <String>]`: The ID of the catalog provided by the app developer in the Microsoft Teams zip app package.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.teams/new-mgteamchanneltab](https://learn.microsoft.com/powershell/module/microsoft.graph.teams/new-mgteamchanneltab)

[https://learn.microsoft.com/graph/api/channel-post-tabs?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/channel-post-tabs?view=graph-rest-1.0)























