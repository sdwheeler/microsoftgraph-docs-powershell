---
external help file: Microsoft.Graph.Beta.Teams-help.xml
Module Name: Microsoft.Graph.Beta.Teams
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/new-mgbetachat
schema: 2.0.0
ms.subservice: teams
---

# New-MgBetaChat

## SYNOPSIS
Create a new chat object.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgChat](/powershell/module/Microsoft.Graph.Teams/New-MgChat?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaChat [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-ChatType <String>]
 [-CreatedBy <IMicrosoftGraphIdentitySet>] [-CreatedDateTime <DateTime>] [-Id <String>]
 [-InstalledApps <IMicrosoftGraphTeamsAppInstallation[]>] [-IsHiddenForAllMembers]
 [-LastMessagePreview <IMicrosoftGraphChatMessageInfo>] [-LastUpdatedDateTime <DateTime>]
 [-Members <IMicrosoftGraphConversationMember[]>] [-Messages <IMicrosoftGraphChatMessage[]>]
 [-OnlineMeetingInfo <IMicrosoftGraphTeamworkOnlineMeetingInfo>]
 [-Operations <IMicrosoftGraphTeamsAsyncOperation[]>]
 [-PermissionGrants <IMicrosoftGraphResourceSpecificPermissionGrant[]>]
 [-PinnedMessages <IMicrosoftGraphPinnedChatMessageInfo[]>] [-Tabs <IMicrosoftGraphTeamsTab[]>]
 [-TenantId <String>] [-Topic <String>] [-Viewpoint <IMicrosoftGraphChatViewpoint>] [-WebUrl <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaChat -BodyParameter <IMicrosoftGraphChat> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new chat object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Chat.Create, Chat.ReadWrite,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Chat.Create,  |

## EXAMPLES
### Example 1: Create a one-on-one chat

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	chatType = "oneOnOne"
	members = @(
		@{
			"@odata.type" = "#microsoft.graph.aadUserConversationMember"
			roles = @(
			"owner"
		)
		"user@odata.bind" = "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
	}
	@{
		"@odata.type" = "#microsoft.graph.aadUserConversationMember"
		roles = @(
		"owner"
	)
	"user@odata.bind" = "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
}
)
}

New-MgBetaChat -BodyParameter $params

```
This example will create a one-on-one chat

### Example 2: Create a group chat

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	chatType = "group"
	topic = "Group chat title"
	members = @(
		@{
			"@odata.type" = "#microsoft.graph.aadUserConversationMember"
			roles = @(
			"owner"
		)
		"user@odata.bind" = "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"
	}
	@{
		"@odata.type" = "#microsoft.graph.aadUserConversationMember"
		roles = @(
		"owner"
	)
	"user@odata.bind" = "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"
}
@{
	"@odata.type" = "#microsoft.graph.aadUserConversationMember"
	roles = @(
	"owner"
)
"user@odata.bind" = "https://graph.microsoft.com/beta/users('3626a173-f2bc-4883-bcf7-01514c3bfb82')"
}
)
}

New-MgBetaChat -BodyParameter $params

```
This example will create a group chat

### Example 3: Create a one-on-one chat with installed apps

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	chatType = "oneOnOne"
	members = @(
		@{
			"@odata.type" = "#microsoft.graph.aadUserConversationMember"
			roles = @(
			"owner"
		)
		"user@odata.bind" = "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
	}
	@{
		"@odata.type" = "#microsoft.graph.aadUserConversationMember"
		roles = @(
		"owner"
	)
	"user@odata.bind" = "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
}
)
installedApps = @(
@{
	"teamsApp@odata.bind" = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4"
}
)
}

New-MgBetaChat -BodyParameter $params

```
This example will create a one-on-one chat with installed apps

### Example 4: Create a one-on-one chat using user principal name

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	chatType = "oneOnOne"
	members = @(
		@{
			"@odata.type" = "#microsoft.graph.aadUserConversationMember"
			roles = @(
			"owner"
		)
		"user@odata.bind" = "https://graph.microsoft.com/beta/users('jacob@contoso.com')"
	}
	@{
		"@odata.type" = "#microsoft.graph.aadUserConversationMember"
		roles = @(
		"owner"
	)
	"user@odata.bind" = "https://graph.microsoft.com/beta/users('alex@contoso.com')"
}
)
}

New-MgBetaChat -BodyParameter $params

```
This example will create a one-on-one chat using user principal name

### Example 5: Create a group chat with in-tenant guest

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	chatType = "group"
	topic = "Group chat title"
	members = @(
		@{
			"@odata.type" = "#microsoft.graph.aadUserConversationMember"
			roles = @(
			"owner"
		)
		"user@odata.bind" = "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"
	}
	@{
		"@odata.type" = "#microsoft.graph.aadUserConversationMember"
		roles = @(
		"owner"
	)
	"user@odata.bind" = "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"
}
@{
	"@odata.type" = "#microsoft.graph.aadUserConversationMember"
	roles = @(
	"guest"
)
"user@odata.bind" = "https://graph.microsoft.com/beta/users('8ba98gf6-7fc2-4eb2-c7f2-aef9f21fd98g')"
}
)
}

New-MgBetaChat -BodyParameter $params

```
This example will create a group chat with in-tenant guest

### Example 6: Create a one-on-one chat with a federated user (outside of own organization)

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	chatType = "oneOnOne"
	members = @(
		@{
			"@odata.type" = "#microsoft.graph.aadUserConversationMember"
			roles = @(
			"owner"
		)
		"user@odata.bind" = "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
	}
	@{
		"@odata.type" = "#microsoft.graph.aadUserConversationMember"
		roles = @(
		"owner"
	)
	"user@odata.bind" = "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
	tenantId = "4dc1fe35-8ac6-4f0d-904a-7ebcd364bea1"
}
)
}

New-MgBetaChat -BodyParameter $params

```
This example will create a one-on-one chat with a federated user (outside of own organization)


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
chat
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphChat
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChatType
chatType

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

### -CreatedBy
identitySet
To construct, see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
Date and time at which the chat was created.
Read-only.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
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
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InstalledApps
A collection of all the apps in the chat.
Nullable.
To construct, see NOTES section for INSTALLEDAPPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsAppInstallation[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsHiddenForAllMembers
Indicates whether the chat is hidden for all its members.
Read-only.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastMessagePreview
chatMessageInfo
To construct, see NOTES section for LASTMESSAGEPREVIEW properties and create a hash table.

```yaml
Type: IMicrosoftGraphChatMessageInfo
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastUpdatedDateTime
Date and time at which the chat was renamed or list of members were last changed.
Read-only.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Members
A collection of all the members in the chat.
Nullable.
To construct, see NOTES section for MEMBERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphConversationMember[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Messages
A collection of all the messages in the chat.
Nullable.
To construct, see NOTES section for MESSAGES properties and create a hash table.

```yaml
Type: IMicrosoftGraphChatMessage[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OnlineMeetingInfo
teamworkOnlineMeetingInfo
To construct, see NOTES section for ONLINEMEETINGINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamworkOnlineMeetingInfo
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Operations
A collection of all the Teams async operations that ran or are running on the chat.
Nullable.
To construct, see NOTES section for OPERATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsAsyncOperation[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PermissionGrants
A collection of permissions granted to apps for the chat.
To construct, see NOTES section for PERMISSIONGRANTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphResourceSpecificPermissionGrant[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinnedMessages
A collection of all the pinned messages in the chat.
Nullable.
To construct, see NOTES section for PINNEDMESSAGES properties and create a hash table.

```yaml
Type: IMicrosoftGraphPinnedChatMessageInfo[]
Parameter Sets: CreateExpanded
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

### -Tabs
A collection of all the tabs in the chat.
Nullable.
To construct, see NOTES section for TABS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsTab[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TenantId
The identifier of the tenant in which the chat was created.
Read-only.

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

### -Topic
(Optional) Subject or topic for the chat.
Only available for group chats.

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

### -Viewpoint
chatViewpoint
To construct, see NOTES section for VIEWPOINT properties and create a hash table.

```yaml
Type: IMicrosoftGraphChatViewpoint
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebUrl
The URL for the chat in Microsoft Teams.
The URL should be treated as an opaque blob, and not parsed.
Read-only.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphChat
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphChat
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphChat>`: chat
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ChatType <String>]`: chatType
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CreatedDateTime <DateTime?>]`: Date and time at which the chat was created.
Read-only.
  - `[InstalledApps <IMicrosoftGraphTeamsAppInstallation- `[]`>]`: A collection of all the apps in the chat.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ConsentedPermissionSet <IMicrosoftGraphTeamsAppPermissionSet>]`: teamsAppPermissionSet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ResourceSpecificPermissions <IMicrosoftGraphTeamsAppResourceSpecificPermission- `[]`>]`: A collection of resource-specific permissions.
        - `[PermissionType <String>]`: teamsAppResourceSpecificPermissionType
        - `[PermissionValue <String>]`: The name of the resource-specific permission.
    - `[ScopeInfo <IMicrosoftGraphTeamsAppInstallationScopeInfo>]`: teamsAppInstallationScopeInfo
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Scope <String>]`: teamsAppInstallationScopes
    - `[TeamsApp <IMicrosoftGraphTeamsApp>]`: teamsApp
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AppDefinitions <IMicrosoftGraphTeamsAppDefinition- `[]`>]`: The details for each version of the app.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[AllowedInstallationScopes <String>]`: teamsAppInstallationScopes
        - `[Authorization <IMicrosoftGraphTeamsAppAuthorization>]`: teamsAppAuthorization
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[ClientAppId <String>]`: The registration ID of the Microsoft Entra app ID associated with the teamsApp.
          - `[RequiredPermissionSet <IMicrosoftGraphTeamsAppPermissionSet>]`: teamsAppPermissionSet
        - `[AzureAdAppId <String>]`: The WebApplicationInfo.Id from the Teams app manifest.
        - `[Bot <IMicrosoftGraphTeamworkBot>]`: teamworkBot
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[ColorIcon <IMicrosoftGraphTeamsAppIcon>]`: teamsAppIcon
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
          - `[HostedContent <IMicrosoftGraphTeamworkHostedContent>]`: teamworkHostedContent
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[Id <String>]`: The unique identifier for an entity.
Read-only.
            - `[ContentBytes <Byte- `[]`>]`: Write only.
Bytes for the hosted content (such as images).
            - `[ContentType <String>]`: Write only.
Content type, such as image/png, image/jpg.
          - `[WebUrl <String>]`: The web URL that can be used for downloading the image.
        - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[DashboardCards <IMicrosoftGraphTeamsAppDashboardCardDefinition- `[]`>]`: Dashboard cards specified in the Teams app manifest.
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
          - `[ContentSource <IMicrosoftGraphTeamsAppDashboardCardContentSource>]`: teamsAppDashboardCardContentSource
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[BotConfiguration <IMicrosoftGraphTeamsAppDashboardCardBotConfiguration>]`: teamsAppDashboardCardBotConfiguration
              - `[(Any) <Object>]`: This indicates any property can be added to this object.
              - `[BotId <String>]`: The ID (usually a GUID) of the bot associated with the specific teamsAppDefinition.
This is a unique app ID for the bot as registered with the Bot Framework.
            - `[SourceType <String>]`: teamsAppDashboardCardSourceType
          - `[DefaultSize <String>]`: teamsAppDashboardCardSize
          - `[Description <String>]`: The description for the card.
Required.
          - `[DisplayName <String>]`: The name of the card.
Required.
          - `[Icon <IMicrosoftGraphTeamsAppDashboardCardIcon>]`: teamsAppDashboardCardIcon
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[IconUrl <String>]`: The icon for the card, displayed in the toolbox and card bar, is represented as a URL.
The preferred size for raster images is 28x28 pixels.
If this property has a value, the officeFabricIconFontName property is ignored.
            - `[OfficeUiFabricIconName <String>]`: The friendly name of the Office UI Fabric/Fluent UI icon for the card that is used when the iconUrl property isn't specified.
For example, 'officeUIFabricIconName': 'Search'.
          - `[PickerGroupId <String>]`: ID for the group in the card picker.
Required.
        - `[Description <String>]`: 
        - `[DisplayName <String>]`: The name of the app provided by the app developer.
        - `[LastModifiedDateTime <DateTime?>]`: 
        - `[OutlineIcon <IMicrosoftGraphTeamsAppIcon>]`: teamsAppIcon
        - `[PublishingState <String>]`: teamsAppPublishingState
        - `[Shortdescription <String>]`: 
        - `[TeamsAppId <String>]`: The ID from the Teams app manifest.
        - `[Version <String>]`: The version number of the application.
      - `[DisplayName <String>]`: The name of the catalog app provided by the app developer in the Microsoft Teams zip app package.
      - `[DistributionMethod <String>]`: teamsAppDistributionMethod
      - `[ExternalId <String>]`: The ID of the catalog provided by the app developer in the Microsoft Teams zip app package.
    - `[TeamsAppDefinition <IMicrosoftGraphTeamsAppDefinition>]`: teamsAppDefinition
  - `[IsHiddenForAllMembers <Boolean?>]`: Indicates whether the chat is hidden for all its members.
Read-only.
  - `[LastMessagePreview <IMicrosoftGraphChatMessageInfo>]`: chatMessageInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Body <IMicrosoftGraphItemBody>]`: itemBody
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Content <String>]`: The content of the item.
      - `[ContentType <String>]`: bodyType
    - `[CreatedDateTime <DateTime?>]`: Date time object representing the time at which message was created.
    - `[EventDetail <IMicrosoftGraphEventMessageDetail>]`: eventMessageDetail
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[From <IMicrosoftGraphChatMessageFromIdentitySet>]`: chatMessageFromIdentitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[IsDeleted <Boolean?>]`: If set to true, the original message has been deleted.
    - `[MessageType <String>]`: chatMessageType
  - `[LastUpdatedDateTime <DateTime?>]`: Date and time at which the chat was renamed or list of members were last changed.
Read-only.
  - `[Members <IMicrosoftGraphConversationMember- `[]`>]`: A collection of all the members in the chat.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: The display name of the user.
    - `[Roles <String- `[]`>]`: The roles for that user.
This property contains additional qualifiers only when relevant - for example, if the member has owner privileges, the roles property contains owner as one of the values.
Similarly, if the member is an in-tenant guest, the roles property contains guest as one of the values.
A basic member should not have any values specified in the roles property.
An Out-of-tenant external member is assigned the owner role.
    - `[VisibleHistoryStartDateTime <DateTime?>]`: The timestamp denoting how far back a conversation's history is shared with the conversation member.
This property is settable only for members of a chat.
  - `[Messages <IMicrosoftGraphChatMessage- `[]`>]`: A collection of all the messages in the chat.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Attachments <IMicrosoftGraphChatMessageAttachment- `[]`>]`: References to attached objects like files, tabs, meetings etc.
      - `[Content <String>]`: The content of the attachment.
If the attachment is a rich card, set the property to the rich card object.
This property and contentUrl are mutually exclusive.
      - `[ContentType <String>]`: The media type of the content attachment.
The possible values are: reference: The attachment is a link to another file.
Populate the contentURL with the link to the object.forwardedMessageReference: The attachment is a reference to a forwarded message.
Populate the content with the original message context.Any contentType that is supported by the Bot Framework's Attachment object.application/vnd.microsoft.card.codesnippet: Either a code snippet or place holder.
application/vnd.microsoft.card.announcement: An announcement header.
application/vnd.microsoft.card.fluidEmbedCard: A Microsoft Loop component.
      - `[ContentUrl <String>]`: The URL for the content of the attachment.
      - `[Id <String>]`: Read-only.
The unique ID of the attachment.
      - `[Name <String>]`: Name of the attachment.
      - `[TeamsAppId <String>]`: The ID of the Teams app that is associated with the attachment.
The property is used to attribute a Teams message card to the specified app.
      - `[ThumbnailUrl <String>]`: The URL to a thumbnail image that the channel can use if it supports using an alternative, smaller form of content or contentUrl.
For example, if you set contentType to application/word and set contentUrl to the location of the Word document, you might include a thumbnail image that represents the document.
The channel could display the thumbnail image instead of the document.
When the user selects the image, the channel would open the document.
    - `[Body <IMicrosoftGraphItemBody>]`: itemBody
    - `[ChannelIdentity <IMicrosoftGraphChannelIdentity>]`: channelIdentity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ChannelId <String>]`: The identity of the channel in which the message was posted.
      - `[TeamId <String>]`: The identity of the team in which the message was posted.
    - `[ChatId <String>]`: If the message was sent in a chat, represents the identity of the chat.
    - `[CreatedDateTime <DateTime?>]`: Timestamp of when the chat message was created.
    - `[DeletedDateTime <DateTime?>]`: Read only.
Timestamp at which the chat message was deleted, or null if not deleted.
    - `[Etag <String>]`: Read-only.
Version number of the chat message.
    - `[EventDetail <IMicrosoftGraphEventMessageDetail>]`: eventMessageDetail
    - `[From <IMicrosoftGraphChatMessageFromIdentitySet>]`: chatMessageFromIdentitySet
    - `[HostedContents <IMicrosoftGraphChatMessageHostedContent- `[]`>]`: Content in a message hosted by Microsoft Teams - for example, images or code snippets.
      - `[ContentBytes <Byte- `[]`>]`: Write only.
Bytes for the hosted content (such as images).
      - `[ContentType <String>]`: Write only.
Content type, such as image/png, image/jpg.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Importance <String>]`: chatMessageImportance
    - `[LastEditedDateTime <DateTime?>]`: Read only.
Timestamp when edits to the chat message were made.
Triggers an 'Edited' flag in the Teams UI.
If no edits are made the value is null.
    - `[LastModifiedDateTime <DateTime?>]`: Read only.
Timestamp when the chat message is created (initial setting) or modified, including when a reaction is added or removed.
    - `[Locale <String>]`: Locale of the chat message set by the client.
Always set to en-us.
    - `[Mentions <IMicrosoftGraphChatMessageMention- `[]`>]`: List of entities mentioned in the chat message.
Supported entities are: user, bot, team, channel, chat, and tag.
      - `[Id <Int32?>]`: Index of an entity being mentioned in the specified chatMessage.
Matches the {index} value in the corresponding `<at id='{index}'>` tag in the message body.
      - `[MentionText <String>]`: String used to represent the mention.
For example, a user's display name, a team name.
      - `[Mentioned <IMicrosoftGraphChatMessageMentionedIdentitySet>]`: chatMessageMentionedIdentitySet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[Device <IMicrosoftGraphIdentity>]`: identity
        - `[User <IMicrosoftGraphIdentity>]`: identity
        - `[Conversation <IMicrosoftGraphTeamworkConversationIdentity>]`: teamworkConversationIdentity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
          - `[Id <String>]`: The identifier of the identity.
This property is read-only.
          - `[ConversationIdentityType <String>]`: teamworkConversationIdentityType
        - `[Tag <IMicrosoftGraphTeamworkTagIdentity>]`: teamworkTagIdentity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
          - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[MessageHistory <IMicrosoftGraphChatMessageHistoryItem- `[]`>]`: List of activity history of a message item, including modification time and actions, such as reactionAdded, reactionRemoved, or reaction changes, on the message.
      - `[Actions <String>]`: chatMessageActions
      - `[ModifiedDateTime <DateTime?>]`: The date and time when the message was modified.
      - `[Reaction <IMicrosoftGraphChatMessageReaction>]`: chatMessageReaction
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[CreatedDateTime <DateTime?>]`: The timestamp type represents date and time information using ISO 8601 format and is always in UTC.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        - `[DisplayName <String>]`: The name of the reaction.
        - `[ReactionContentUrl <String>]`: The hosted content URL for the custom reaction type.
        - `[ReactionType <String>]`: The reaction type.
Supported values include Unicode characters, custom, and some backward-compatible reaction types, such as like, angry, sad, laugh, heart, and surprised.
        - `[User <IMicrosoftGraphChatMessageReactionIdentitySet>]`: chatMessageReactionIdentitySet
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Application <IMicrosoftGraphIdentity>]`: identity
          - `[Device <IMicrosoftGraphIdentity>]`: identity
          - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[MessageType <String>]`: chatMessageType
    - `[OnBehalfOf <IMicrosoftGraphChatMessageFromIdentitySet>]`: chatMessageFromIdentitySet
    - `[PolicyViolation <IMicrosoftGraphChatMessagePolicyViolation>]`: chatMessagePolicyViolation
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DlpAction <String>]`: chatMessagePolicyViolationDlpActionTypes
      - `[JustificationText <String>]`: Justification text provided by the sender of the message when overriding a policy violation.
      - `[PolicyTip <IMicrosoftGraphChatMessagePolicyViolationPolicyTip>]`: chatMessagePolicyViolationPolicyTip
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[ComplianceUrl <String>]`: The URL a user can visit to read about the data loss prevention policies for the organization.
(ie, policies about what users shouldn't say in chats)
        - `[GeneralText <String>]`: Explanatory text shown to the sender of the message.
        - `[MatchedConditionDescriptions <String- `[]`>]`: The list of improper data in the message that was detected by the data loss prevention app.
Each DLP app defines its own conditions, examples include 'Credit Card Number' and 'Social Security Number'.
      - `[UserAction <String>]`: chatMessagePolicyViolationUserActionTypes
      - `[VerdictDetails <String>]`: chatMessagePolicyViolationVerdictDetailsTypes
    - `[Reactions <IMicrosoftGraphChatMessageReaction- `[]`>]`: Reactions for this chat message (for example, Like).
    - `[Replies <IMicrosoftGraphChatMessage- `[]`>]`: Replies for a specified message.
Supports $expand for channel messages.
    - `[ReplyToId <String>]`: Read-only.
ID of the parent chat message or root chat message of the thread.
(Only applies to chat messages in channels, not chats.)
    - `[Subject <String>]`: The subject of the chat message, in plaintext.
    - `[Summary <String>]`: Summary text of the chat message that could be used for push notifications and summary views or fall back views.
Only applies to channel chat messages, not chat messages in a chat.
    - `[WebUrl <String>]`: Read-only.
Link to the message in Microsoft Teams.
  - `[OnlineMeetingInfo <IMicrosoftGraphTeamworkOnlineMeetingInfo>]`: teamworkOnlineMeetingInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CalendarEventId <String>]`: The identifier of the calendar event associated with the meeting.
    - `[JoinWebUrl <String>]`: The URL which can be clicked on to join or uniquely identify the meeting.
    - `[Organizer <IMicrosoftGraphTeamworkUserIdentity>]`: teamworkUserIdentity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
      - `[UserIdentityType <String>]`: teamworkUserIdentityType
  - `[Operations <IMicrosoftGraphTeamsAsyncOperation- `[]`>]`: A collection of all the Teams async operations that ran or are running on the chat.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AttemptsCount <Int32?>]`: Number of times the operation was attempted before being marked successful or failed.
    - `[CreatedDateTime <DateTime?>]`: Time when the operation was created.
    - `[Error <IMicrosoftGraphOperationError>]`: operationError
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Code <String>]`: Operation error code.
      - `[Message <String>]`: Operation error message.
    - `[LastActionDateTime <DateTime?>]`: Time when the async operation was last updated.
    - `[OperationType <String>]`: teamsAsyncOperationType
    - `[Status <String>]`: teamsAsyncOperationStatus
    - `[TargetResourceId <String>]`: The ID of the object that's created or modified as result of this async operation, typically a team.
    - `[TargetResourceLocation <String>]`: The location of the object that's created or modified as result of this async operation.
This URL should be treated as an opaque value and not parsed into its component paths.
  - `[PermissionGrants <IMicrosoftGraphResourceSpecificPermissionGrant- `[]`>]`: A collection of permissions granted to apps for the chat.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ClientAppId <String>]`: ID of the service principal of the Microsoft Entra app that has been granted access.
Read-only.
    - `[ClientId <String>]`: ID of the Microsoft Entra app that has been granted access.
Read-only.
    - `[Permission <String>]`: The name of the resource-specific permission.
Read-only.
    - `[PermissionType <String>]`: The type of permission.
Possible values are: Application, Delegated.
Read-only.
    - `[ResourceAppId <String>]`: ID of the Microsoft Entra app that is hosting the resource.
Read-only.
  - `[PinnedMessages <IMicrosoftGraphPinnedChatMessageInfo- `[]`>]`: A collection of all the pinned messages in the chat.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Message <IMicrosoftGraphChatMessage>]`: chatMessage
  - `[Tabs <IMicrosoftGraphTeamsTab- `[]`>]`: A collection of all the tabs in the chat.
Nullable.
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
    - `[MessageId <String>]`: 
    - `[SortOrderIndex <String>]`: Index of the order used for sorting tabs.
    - `[TeamsApp <IMicrosoftGraphTeamsApp>]`: teamsApp
    - `[TeamsAppId <String>]`: App definition identifier of the tab.
This value can't be changed after tab creation.
Because this property is deprecated, we recommend expanding teamsApp to retrieve the application that is linked to the tab.
    - `[WebUrl <String>]`: Deep link URL of the tab instance.
Read only.
  - `[TenantId <String>]`: The identifier of the tenant in which the chat was created.
Read-only.
  - `[Topic <String>]`: (Optional) Subject or topic for the chat.
Only available for group chats.
  - `[Viewpoint <IMicrosoftGraphChatViewpoint>]`: chatViewpoint
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsHidden <Boolean?>]`: Indicates whether the chat is hidden for the current user.
    - `[LastMessageReadDateTime <DateTime?>]`: Represents the dateTime up until which the current user has read chatMessages in a specific chat.
  - `[WebUrl <String>]`: The URL for the chat in Microsoft Teams.
The URL should be treated as an opaque blob, and not parsed.
Read-only.

CREATEDBY `<IMicrosoftGraphIdentitySet>`: identitySet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Application <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
    - `[Id <String>]`: The identifier of the identity.
This property is read-only.
  - `[Device <IMicrosoftGraphIdentity>]`: identity
  - `[User <IMicrosoftGraphIdentity>]`: identity

INSTALLEDAPPS `<IMicrosoftGraphTeamsAppInstallation- `[]`>`: A collection of all the apps in the chat.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ConsentedPermissionSet <IMicrosoftGraphTeamsAppPermissionSet>]`: teamsAppPermissionSet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ResourceSpecificPermissions <IMicrosoftGraphTeamsAppResourceSpecificPermission- `[]`>]`: A collection of resource-specific permissions.
      - `[PermissionType <String>]`: teamsAppResourceSpecificPermissionType
      - `[PermissionValue <String>]`: The name of the resource-specific permission.
  - `[ScopeInfo <IMicrosoftGraphTeamsAppInstallationScopeInfo>]`: teamsAppInstallationScopeInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Scope <String>]`: teamsAppInstallationScopes
  - `[TeamsApp <IMicrosoftGraphTeamsApp>]`: teamsApp
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppDefinitions <IMicrosoftGraphTeamsAppDefinition- `[]`>]`: The details for each version of the app.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AllowedInstallationScopes <String>]`: teamsAppInstallationScopes
      - `[Authorization <IMicrosoftGraphTeamsAppAuthorization>]`: teamsAppAuthorization
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[ClientAppId <String>]`: The registration ID of the Microsoft Entra app ID associated with the teamsApp.
        - `[RequiredPermissionSet <IMicrosoftGraphTeamsAppPermissionSet>]`: teamsAppPermissionSet
      - `[AzureAdAppId <String>]`: The WebApplicationInfo.Id from the Teams app manifest.
      - `[Bot <IMicrosoftGraphTeamworkBot>]`: teamworkBot
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ColorIcon <IMicrosoftGraphTeamsAppIcon>]`: teamsAppIcon
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[HostedContent <IMicrosoftGraphTeamworkHostedContent>]`: teamworkHostedContent
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
          - `[ContentBytes <Byte- `[]`>]`: Write only.
Bytes for the hosted content (such as images).
          - `[ContentType <String>]`: Write only.
Content type, such as image/png, image/jpg.
        - `[WebUrl <String>]`: The web URL that can be used for downloading the image.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Application <IMicrosoftGraphIdentity>]`: identity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
          - `[Id <String>]`: The identifier of the identity.
This property is read-only.
        - `[Device <IMicrosoftGraphIdentity>]`: identity
        - `[User <IMicrosoftGraphIdentity>]`: identity
      - `[DashboardCards <IMicrosoftGraphTeamsAppDashboardCardDefinition- `[]`>]`: Dashboard cards specified in the Teams app manifest.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[ContentSource <IMicrosoftGraphTeamsAppDashboardCardContentSource>]`: teamsAppDashboardCardContentSource
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[BotConfiguration <IMicrosoftGraphTeamsAppDashboardCardBotConfiguration>]`: teamsAppDashboardCardBotConfiguration
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[BotId <String>]`: The ID (usually a GUID) of the bot associated with the specific teamsAppDefinition.
This is a unique app ID for the bot as registered with the Bot Framework.
          - `[SourceType <String>]`: teamsAppDashboardCardSourceType
        - `[DefaultSize <String>]`: teamsAppDashboardCardSize
        - `[Description <String>]`: The description for the card.
Required.
        - `[DisplayName <String>]`: The name of the card.
Required.
        - `[Icon <IMicrosoftGraphTeamsAppDashboardCardIcon>]`: teamsAppDashboardCardIcon
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[IconUrl <String>]`: The icon for the card, displayed in the toolbox and card bar, is represented as a URL.
The preferred size for raster images is 28x28 pixels.
If this property has a value, the officeFabricIconFontName property is ignored.
          - `[OfficeUiFabricIconName <String>]`: The friendly name of the Office UI Fabric/Fluent UI icon for the card that is used when the iconUrl property isn't specified.
For example, 'officeUIFabricIconName': 'Search'.
        - `[PickerGroupId <String>]`: ID for the group in the card picker.
Required.
      - `[Description <String>]`: 
      - `[DisplayName <String>]`: The name of the app provided by the app developer.
      - `[LastModifiedDateTime <DateTime?>]`: 
      - `[OutlineIcon <IMicrosoftGraphTeamsAppIcon>]`: teamsAppIcon
      - `[PublishingState <String>]`: teamsAppPublishingState
      - `[Shortdescription <String>]`: 
      - `[TeamsAppId <String>]`: The ID from the Teams app manifest.
      - `[Version <String>]`: The version number of the application.
    - `[DisplayName <String>]`: The name of the catalog app provided by the app developer in the Microsoft Teams zip app package.
    - `[DistributionMethod <String>]`: teamsAppDistributionMethod
    - `[ExternalId <String>]`: The ID of the catalog provided by the app developer in the Microsoft Teams zip app package.
  - `[TeamsAppDefinition <IMicrosoftGraphTeamsAppDefinition>]`: teamsAppDefinition

LASTMESSAGEPREVIEW `<IMicrosoftGraphChatMessageInfo>`: chatMessageInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Body <IMicrosoftGraphItemBody>]`: itemBody
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Content <String>]`: The content of the item.
    - `[ContentType <String>]`: bodyType
  - `[CreatedDateTime <DateTime?>]`: Date time object representing the time at which message was created.
  - `[EventDetail <IMicrosoftGraphEventMessageDetail>]`: eventMessageDetail
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[From <IMicrosoftGraphChatMessageFromIdentitySet>]`: chatMessageFromIdentitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[IsDeleted <Boolean?>]`: If set to true, the original message has been deleted.
  - `[MessageType <String>]`: chatMessageType

MEMBERS `<IMicrosoftGraphConversationMember- `[]`>`: A collection of all the members in the chat.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The display name of the user.
  - `[Roles <String- `[]`>]`: The roles for that user.
This property contains additional qualifiers only when relevant - for example, if the member has owner privileges, the roles property contains owner as one of the values.
Similarly, if the member is an in-tenant guest, the roles property contains guest as one of the values.
A basic member should not have any values specified in the roles property.
An Out-of-tenant external member is assigned the owner role.
  - `[VisibleHistoryStartDateTime <DateTime?>]`: The timestamp denoting how far back a conversation's history is shared with the conversation member.
This property is settable only for members of a chat.

MESSAGES `<IMicrosoftGraphChatMessage- `[]`>`: A collection of all the messages in the chat.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Attachments <IMicrosoftGraphChatMessageAttachment- `[]`>]`: References to attached objects like files, tabs, meetings etc.
    - `[Content <String>]`: The content of the attachment.
If the attachment is a rich card, set the property to the rich card object.
This property and contentUrl are mutually exclusive.
    - `[ContentType <String>]`: The media type of the content attachment.
The possible values are: reference: The attachment is a link to another file.
Populate the contentURL with the link to the object.forwardedMessageReference: The attachment is a reference to a forwarded message.
Populate the content with the original message context.Any contentType that is supported by the Bot Framework's Attachment object.application/vnd.microsoft.card.codesnippet: Either a code snippet or place holder.
application/vnd.microsoft.card.announcement: An announcement header.
application/vnd.microsoft.card.fluidEmbedCard: A Microsoft Loop component.
    - `[ContentUrl <String>]`: The URL for the content of the attachment.
    - `[Id <String>]`: Read-only.
The unique ID of the attachment.
    - `[Name <String>]`: Name of the attachment.
    - `[TeamsAppId <String>]`: The ID of the Teams app that is associated with the attachment.
The property is used to attribute a Teams message card to the specified app.
    - `[ThumbnailUrl <String>]`: The URL to a thumbnail image that the channel can use if it supports using an alternative, smaller form of content or contentUrl.
For example, if you set contentType to application/word and set contentUrl to the location of the Word document, you might include a thumbnail image that represents the document.
The channel could display the thumbnail image instead of the document.
When the user selects the image, the channel would open the document.
  - `[Body <IMicrosoftGraphItemBody>]`: itemBody
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Content <String>]`: The content of the item.
    - `[ContentType <String>]`: bodyType
  - `[ChannelIdentity <IMicrosoftGraphChannelIdentity>]`: channelIdentity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ChannelId <String>]`: The identity of the channel in which the message was posted.
    - `[TeamId <String>]`: The identity of the team in which the message was posted.
  - `[ChatId <String>]`: If the message was sent in a chat, represents the identity of the chat.
  - `[CreatedDateTime <DateTime?>]`: Timestamp of when the chat message was created.
  - `[DeletedDateTime <DateTime?>]`: Read only.
Timestamp at which the chat message was deleted, or null if not deleted.
  - `[Etag <String>]`: Read-only.
Version number of the chat message.
  - `[EventDetail <IMicrosoftGraphEventMessageDetail>]`: eventMessageDetail
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[From <IMicrosoftGraphChatMessageFromIdentitySet>]`: chatMessageFromIdentitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[HostedContents <IMicrosoftGraphChatMessageHostedContent- `[]`>]`: Content in a message hosted by Microsoft Teams - for example, images or code snippets.
    - `[ContentBytes <Byte- `[]`>]`: Write only.
Bytes for the hosted content (such as images).
    - `[ContentType <String>]`: Write only.
Content type, such as image/png, image/jpg.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Importance <String>]`: chatMessageImportance
  - `[LastEditedDateTime <DateTime?>]`: Read only.
Timestamp when edits to the chat message were made.
Triggers an 'Edited' flag in the Teams UI.
If no edits are made the value is null.
  - `[LastModifiedDateTime <DateTime?>]`: Read only.
Timestamp when the chat message is created (initial setting) or modified, including when a reaction is added or removed.
  - `[Locale <String>]`: Locale of the chat message set by the client.
Always set to en-us.
  - `[Mentions <IMicrosoftGraphChatMessageMention- `[]`>]`: List of entities mentioned in the chat message.
Supported entities are: user, bot, team, channel, chat, and tag.
    - `[Id <Int32?>]`: Index of an entity being mentioned in the specified chatMessage.
Matches the {index} value in the corresponding `<at id='{index}'>` tag in the message body.
    - `[MentionText <String>]`: String used to represent the mention.
For example, a user's display name, a team name.
    - `[Mentioned <IMicrosoftGraphChatMessageMentionedIdentitySet>]`: chatMessageMentionedIdentitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
      - `[Conversation <IMicrosoftGraphTeamworkConversationIdentity>]`: teamworkConversationIdentity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
        - `[Id <String>]`: The identifier of the identity.
This property is read-only.
        - `[ConversationIdentityType <String>]`: teamworkConversationIdentityType
      - `[Tag <IMicrosoftGraphTeamworkTagIdentity>]`: teamworkTagIdentity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
        - `[Id <String>]`: The identifier of the identity.
This property is read-only.
  - `[MessageHistory <IMicrosoftGraphChatMessageHistoryItem- `[]`>]`: List of activity history of a message item, including modification time and actions, such as reactionAdded, reactionRemoved, or reaction changes, on the message.
    - `[Actions <String>]`: chatMessageActions
    - `[ModifiedDateTime <DateTime?>]`: The date and time when the message was modified.
    - `[Reaction <IMicrosoftGraphChatMessageReaction>]`: chatMessageReaction
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CreatedDateTime <DateTime?>]`: The timestamp type represents date and time information using ISO 8601 format and is always in UTC.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[DisplayName <String>]`: The name of the reaction.
      - `[ReactionContentUrl <String>]`: The hosted content URL for the custom reaction type.
      - `[ReactionType <String>]`: The reaction type.
Supported values include Unicode characters, custom, and some backward-compatible reaction types, such as like, angry, sad, laugh, heart, and surprised.
      - `[User <IMicrosoftGraphChatMessageReactionIdentitySet>]`: chatMessageReactionIdentitySet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[Device <IMicrosoftGraphIdentity>]`: identity
        - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[MessageType <String>]`: chatMessageType
  - `[OnBehalfOf <IMicrosoftGraphChatMessageFromIdentitySet>]`: chatMessageFromIdentitySet
  - `[PolicyViolation <IMicrosoftGraphChatMessagePolicyViolation>]`: chatMessagePolicyViolation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DlpAction <String>]`: chatMessagePolicyViolationDlpActionTypes
    - `[JustificationText <String>]`: Justification text provided by the sender of the message when overriding a policy violation.
    - `[PolicyTip <IMicrosoftGraphChatMessagePolicyViolationPolicyTip>]`: chatMessagePolicyViolationPolicyTip
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ComplianceUrl <String>]`: The URL a user can visit to read about the data loss prevention policies for the organization.
(ie, policies about what users shouldn't say in chats)
      - `[GeneralText <String>]`: Explanatory text shown to the sender of the message.
      - `[MatchedConditionDescriptions <String- `[]`>]`: The list of improper data in the message that was detected by the data loss prevention app.
Each DLP app defines its own conditions, examples include 'Credit Card Number' and 'Social Security Number'.
    - `[UserAction <String>]`: chatMessagePolicyViolationUserActionTypes
    - `[VerdictDetails <String>]`: chatMessagePolicyViolationVerdictDetailsTypes
  - `[Reactions <IMicrosoftGraphChatMessageReaction- `[]`>]`: Reactions for this chat message (for example, Like).
  - `[Replies <IMicrosoftGraphChatMessage- `[]`>]`: Replies for a specified message.
Supports $expand for channel messages.
  - `[ReplyToId <String>]`: Read-only.
ID of the parent chat message or root chat message of the thread.
(Only applies to chat messages in channels, not chats.)
  - `[Subject <String>]`: The subject of the chat message, in plaintext.
  - `[Summary <String>]`: Summary text of the chat message that could be used for push notifications and summary views or fall back views.
Only applies to channel chat messages, not chat messages in a chat.
  - `[WebUrl <String>]`: Read-only.
Link to the message in Microsoft Teams.

ONLINEMEETINGINFO `<IMicrosoftGraphTeamworkOnlineMeetingInfo>`: teamworkOnlineMeetingInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CalendarEventId <String>]`: The identifier of the calendar event associated with the meeting.
  - `[JoinWebUrl <String>]`: The URL which can be clicked on to join or uniquely identify the meeting.
  - `[Organizer <IMicrosoftGraphTeamworkUserIdentity>]`: teamworkUserIdentity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
    - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[UserIdentityType <String>]`: teamworkUserIdentityType

OPERATIONS `<IMicrosoftGraphTeamsAsyncOperation- `[]`>`: A collection of all the Teams async operations that ran or are running on the chat.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AttemptsCount <Int32?>]`: Number of times the operation was attempted before being marked successful or failed.
  - `[CreatedDateTime <DateTime?>]`: Time when the operation was created.
  - `[Error <IMicrosoftGraphOperationError>]`: operationError
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Code <String>]`: Operation error code.
    - `[Message <String>]`: Operation error message.
  - `[LastActionDateTime <DateTime?>]`: Time when the async operation was last updated.
  - `[OperationType <String>]`: teamsAsyncOperationType
  - `[Status <String>]`: teamsAsyncOperationStatus
  - `[TargetResourceId <String>]`: The ID of the object that's created or modified as result of this async operation, typically a team.
  - `[TargetResourceLocation <String>]`: The location of the object that's created or modified as result of this async operation.
This URL should be treated as an opaque value and not parsed into its component paths.

PERMISSIONGRANTS `<IMicrosoftGraphResourceSpecificPermissionGrant- `[]`>`: A collection of permissions granted to apps for the chat.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ClientAppId <String>]`: ID of the service principal of the Microsoft Entra app that has been granted access.
Read-only.
  - `[ClientId <String>]`: ID of the Microsoft Entra app that has been granted access.
Read-only.
  - `[Permission <String>]`: The name of the resource-specific permission.
Read-only.
  - `[PermissionType <String>]`: The type of permission.
Possible values are: Application, Delegated.
Read-only.
  - `[ResourceAppId <String>]`: ID of the Microsoft Entra app that is hosting the resource.
Read-only.

PINNEDMESSAGES `<IMicrosoftGraphPinnedChatMessageInfo- `[]`>`: A collection of all the pinned messages in the chat.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Message <IMicrosoftGraphChatMessage>]`: chatMessage
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Attachments <IMicrosoftGraphChatMessageAttachment- `[]`>]`: References to attached objects like files, tabs, meetings etc.
      - `[Content <String>]`: The content of the attachment.
If the attachment is a rich card, set the property to the rich card object.
This property and contentUrl are mutually exclusive.
      - `[ContentType <String>]`: The media type of the content attachment.
The possible values are: reference: The attachment is a link to another file.
Populate the contentURL with the link to the object.forwardedMessageReference: The attachment is a reference to a forwarded message.
Populate the content with the original message context.Any contentType that is supported by the Bot Framework's Attachment object.application/vnd.microsoft.card.codesnippet: Either a code snippet or place holder.
application/vnd.microsoft.card.announcement: An announcement header.
application/vnd.microsoft.card.fluidEmbedCard: A Microsoft Loop component.
      - `[ContentUrl <String>]`: The URL for the content of the attachment.
      - `[Id <String>]`: Read-only.
The unique ID of the attachment.
      - `[Name <String>]`: Name of the attachment.
      - `[TeamsAppId <String>]`: The ID of the Teams app that is associated with the attachment.
The property is used to attribute a Teams message card to the specified app.
      - `[ThumbnailUrl <String>]`: The URL to a thumbnail image that the channel can use if it supports using an alternative, smaller form of content or contentUrl.
For example, if you set contentType to application/word and set contentUrl to the location of the Word document, you might include a thumbnail image that represents the document.
The channel could display the thumbnail image instead of the document.
When the user selects the image, the channel would open the document.
    - `[Body <IMicrosoftGraphItemBody>]`: itemBody
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Content <String>]`: The content of the item.
      - `[ContentType <String>]`: bodyType
    - `[ChannelIdentity <IMicrosoftGraphChannelIdentity>]`: channelIdentity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ChannelId <String>]`: The identity of the channel in which the message was posted.
      - `[TeamId <String>]`: The identity of the team in which the message was posted.
    - `[ChatId <String>]`: If the message was sent in a chat, represents the identity of the chat.
    - `[CreatedDateTime <DateTime?>]`: Timestamp of when the chat message was created.
    - `[DeletedDateTime <DateTime?>]`: Read only.
Timestamp at which the chat message was deleted, or null if not deleted.
    - `[Etag <String>]`: Read-only.
Version number of the chat message.
    - `[EventDetail <IMicrosoftGraphEventMessageDetail>]`: eventMessageDetail
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[From <IMicrosoftGraphChatMessageFromIdentitySet>]`: chatMessageFromIdentitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
        - `[Id <String>]`: The identifier of the identity.
This property is read-only.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[HostedContents <IMicrosoftGraphChatMessageHostedContent- `[]`>]`: Content in a message hosted by Microsoft Teams - for example, images or code snippets.
      - `[ContentBytes <Byte- `[]`>]`: Write only.
Bytes for the hosted content (such as images).
      - `[ContentType <String>]`: Write only.
Content type, such as image/png, image/jpg.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Importance <String>]`: chatMessageImportance
    - `[LastEditedDateTime <DateTime?>]`: Read only.
Timestamp when edits to the chat message were made.
Triggers an 'Edited' flag in the Teams UI.
If no edits are made the value is null.
    - `[LastModifiedDateTime <DateTime?>]`: Read only.
Timestamp when the chat message is created (initial setting) or modified, including when a reaction is added or removed.
    - `[Locale <String>]`: Locale of the chat message set by the client.
Always set to en-us.
    - `[Mentions <IMicrosoftGraphChatMessageMention- `[]`>]`: List of entities mentioned in the chat message.
Supported entities are: user, bot, team, channel, chat, and tag.
      - `[Id <Int32?>]`: Index of an entity being mentioned in the specified chatMessage.
Matches the {index} value in the corresponding `<at id='{index}'>` tag in the message body.
      - `[MentionText <String>]`: String used to represent the mention.
For example, a user's display name, a team name.
      - `[Mentioned <IMicrosoftGraphChatMessageMentionedIdentitySet>]`: chatMessageMentionedIdentitySet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[Device <IMicrosoftGraphIdentity>]`: identity
        - `[User <IMicrosoftGraphIdentity>]`: identity
        - `[Conversation <IMicrosoftGraphTeamworkConversationIdentity>]`: teamworkConversationIdentity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
          - `[Id <String>]`: The identifier of the identity.
This property is read-only.
          - `[ConversationIdentityType <String>]`: teamworkConversationIdentityType
        - `[Tag <IMicrosoftGraphTeamworkTagIdentity>]`: teamworkTagIdentity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
          - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[MessageHistory <IMicrosoftGraphChatMessageHistoryItem- `[]`>]`: List of activity history of a message item, including modification time and actions, such as reactionAdded, reactionRemoved, or reaction changes, on the message.
      - `[Actions <String>]`: chatMessageActions
      - `[ModifiedDateTime <DateTime?>]`: The date and time when the message was modified.
      - `[Reaction <IMicrosoftGraphChatMessageReaction>]`: chatMessageReaction
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[CreatedDateTime <DateTime?>]`: The timestamp type represents date and time information using ISO 8601 format and is always in UTC.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        - `[DisplayName <String>]`: The name of the reaction.
        - `[ReactionContentUrl <String>]`: The hosted content URL for the custom reaction type.
        - `[ReactionType <String>]`: The reaction type.
Supported values include Unicode characters, custom, and some backward-compatible reaction types, such as like, angry, sad, laugh, heart, and surprised.
        - `[User <IMicrosoftGraphChatMessageReactionIdentitySet>]`: chatMessageReactionIdentitySet
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Application <IMicrosoftGraphIdentity>]`: identity
          - `[Device <IMicrosoftGraphIdentity>]`: identity
          - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[MessageType <String>]`: chatMessageType
    - `[OnBehalfOf <IMicrosoftGraphChatMessageFromIdentitySet>]`: chatMessageFromIdentitySet
    - `[PolicyViolation <IMicrosoftGraphChatMessagePolicyViolation>]`: chatMessagePolicyViolation
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DlpAction <String>]`: chatMessagePolicyViolationDlpActionTypes
      - `[JustificationText <String>]`: Justification text provided by the sender of the message when overriding a policy violation.
      - `[PolicyTip <IMicrosoftGraphChatMessagePolicyViolationPolicyTip>]`: chatMessagePolicyViolationPolicyTip
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[ComplianceUrl <String>]`: The URL a user can visit to read about the data loss prevention policies for the organization.
(ie, policies about what users shouldn't say in chats)
        - `[GeneralText <String>]`: Explanatory text shown to the sender of the message.
        - `[MatchedConditionDescriptions <String- `[]`>]`: The list of improper data in the message that was detected by the data loss prevention app.
Each DLP app defines its own conditions, examples include 'Credit Card Number' and 'Social Security Number'.
      - `[UserAction <String>]`: chatMessagePolicyViolationUserActionTypes
      - `[VerdictDetails <String>]`: chatMessagePolicyViolationVerdictDetailsTypes
    - `[Reactions <IMicrosoftGraphChatMessageReaction- `[]`>]`: Reactions for this chat message (for example, Like).
    - `[Replies <IMicrosoftGraphChatMessage- `[]`>]`: Replies for a specified message.
Supports $expand for channel messages.
    - `[ReplyToId <String>]`: Read-only.
ID of the parent chat message or root chat message of the thread.
(Only applies to chat messages in channels, not chats.)
    - `[Subject <String>]`: The subject of the chat message, in plaintext.
    - `[Summary <String>]`: Summary text of the chat message that could be used for push notifications and summary views or fall back views.
Only applies to channel chat messages, not chat messages in a chat.
    - `[WebUrl <String>]`: Read-only.
Link to the message in Microsoft Teams.

TABS `<IMicrosoftGraphTeamsTab- `[]`>`: A collection of all the tabs in the chat.
Nullable.
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
  - `[MessageId <String>]`: 
  - `[SortOrderIndex <String>]`: Index of the order used for sorting tabs.
  - `[TeamsApp <IMicrosoftGraphTeamsApp>]`: teamsApp
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppDefinitions <IMicrosoftGraphTeamsAppDefinition- `[]`>]`: The details for each version of the app.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AllowedInstallationScopes <String>]`: teamsAppInstallationScopes
      - `[Authorization <IMicrosoftGraphTeamsAppAuthorization>]`: teamsAppAuthorization
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[ClientAppId <String>]`: The registration ID of the Microsoft Entra app ID associated with the teamsApp.
        - `[RequiredPermissionSet <IMicrosoftGraphTeamsAppPermissionSet>]`: teamsAppPermissionSet
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[ResourceSpecificPermissions <IMicrosoftGraphTeamsAppResourceSpecificPermission- `[]`>]`: A collection of resource-specific permissions.
            - `[PermissionType <String>]`: teamsAppResourceSpecificPermissionType
            - `[PermissionValue <String>]`: The name of the resource-specific permission.
      - `[AzureAdAppId <String>]`: The WebApplicationInfo.Id from the Teams app manifest.
      - `[Bot <IMicrosoftGraphTeamworkBot>]`: teamworkBot
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ColorIcon <IMicrosoftGraphTeamsAppIcon>]`: teamsAppIcon
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[HostedContent <IMicrosoftGraphTeamworkHostedContent>]`: teamworkHostedContent
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
          - `[ContentBytes <Byte- `[]`>]`: Write only.
Bytes for the hosted content (such as images).
          - `[ContentType <String>]`: Write only.
Content type, such as image/png, image/jpg.
        - `[WebUrl <String>]`: The web URL that can be used for downloading the image.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Application <IMicrosoftGraphIdentity>]`: identity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
          - `[Id <String>]`: The identifier of the identity.
This property is read-only.
        - `[Device <IMicrosoftGraphIdentity>]`: identity
        - `[User <IMicrosoftGraphIdentity>]`: identity
      - `[DashboardCards <IMicrosoftGraphTeamsAppDashboardCardDefinition- `[]`>]`: Dashboard cards specified in the Teams app manifest.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[ContentSource <IMicrosoftGraphTeamsAppDashboardCardContentSource>]`: teamsAppDashboardCardContentSource
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[BotConfiguration <IMicrosoftGraphTeamsAppDashboardCardBotConfiguration>]`: teamsAppDashboardCardBotConfiguration
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[BotId <String>]`: The ID (usually a GUID) of the bot associated with the specific teamsAppDefinition.
This is a unique app ID for the bot as registered with the Bot Framework.
          - `[SourceType <String>]`: teamsAppDashboardCardSourceType
        - `[DefaultSize <String>]`: teamsAppDashboardCardSize
        - `[Description <String>]`: The description for the card.
Required.
        - `[DisplayName <String>]`: The name of the card.
Required.
        - `[Icon <IMicrosoftGraphTeamsAppDashboardCardIcon>]`: teamsAppDashboardCardIcon
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[IconUrl <String>]`: The icon for the card, displayed in the toolbox and card bar, is represented as a URL.
The preferred size for raster images is 28x28 pixels.
If this property has a value, the officeFabricIconFontName property is ignored.
          - `[OfficeUiFabricIconName <String>]`: The friendly name of the Office UI Fabric/Fluent UI icon for the card that is used when the iconUrl property isn't specified.
For example, 'officeUIFabricIconName': 'Search'.
        - `[PickerGroupId <String>]`: ID for the group in the card picker.
Required.
      - `[Description <String>]`: 
      - `[DisplayName <String>]`: The name of the app provided by the app developer.
      - `[LastModifiedDateTime <DateTime?>]`: 
      - `[OutlineIcon <IMicrosoftGraphTeamsAppIcon>]`: teamsAppIcon
      - `[PublishingState <String>]`: teamsAppPublishingState
      - `[Shortdescription <String>]`: 
      - `[TeamsAppId <String>]`: The ID from the Teams app manifest.
      - `[Version <String>]`: The version number of the application.
    - `[DisplayName <String>]`: The name of the catalog app provided by the app developer in the Microsoft Teams zip app package.
    - `[DistributionMethod <String>]`: teamsAppDistributionMethod
    - `[ExternalId <String>]`: The ID of the catalog provided by the app developer in the Microsoft Teams zip app package.
  - `[TeamsAppId <String>]`: App definition identifier of the tab.
This value can't be changed after tab creation.
Because this property is deprecated, we recommend expanding teamsApp to retrieve the application that is linked to the tab.
  - `[WebUrl <String>]`: Deep link URL of the tab instance.
Read only.

VIEWPOINT `<IMicrosoftGraphChatViewpoint>`: chatViewpoint
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsHidden <Boolean?>]`: Indicates whether the chat is hidden for the current user.
  - `[LastMessageReadDateTime <DateTime?>]`: Represents the dateTime up until which the current user has read chatMessages in a specific chat.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/new-mgbetachat](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/new-mgbetachat)

[https://learn.microsoft.com/graph/api/chat-post?view=graph-rest-beta](https://learn.microsoft.com/graph/api/chat-post?view=graph-rest-beta)























