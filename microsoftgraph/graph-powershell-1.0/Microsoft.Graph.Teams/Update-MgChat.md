---
external help file: Microsoft.Graph.Teams-help.xml
Module Name: Microsoft.Graph.Teams
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.teams/update-mgchat
schema: 2.0.0
ms.subservice: teams
---

# Update-MgChat

## SYNOPSIS
Update the properties of a chat object.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaChat](/powershell/module/Microsoft.Graph.Beta.Teams/Update-MgBetaChat?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgChat -ChatId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-ChatType <String>] [-CreatedDateTime <DateTime>] [-Id <String>]
 [-InstalledApps <IMicrosoftGraphTeamsAppInstallation[]>] [-IsHiddenForAllMembers]
 [-LastMessagePreview <IMicrosoftGraphChatMessageInfo>] [-LastUpdatedDateTime <DateTime>]
 [-Members <IMicrosoftGraphConversationMember[]>] [-Messages <IMicrosoftGraphChatMessage[]>]
 [-OnlineMeetingInfo <IMicrosoftGraphTeamworkOnlineMeetingInfo>]
 [-PermissionGrants <IMicrosoftGraphResourceSpecificPermissionGrant[]>]
 [-PinnedMessages <IMicrosoftGraphPinnedChatMessageInfo[]>] [-Tabs <IMicrosoftGraphTeamsTab[]>]
 [-TenantId <String>] [-Topic <String>] [-Viewpoint <IMicrosoftGraphChatViewpoint>] [-WebUrl <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgChat -ChatId <String> -BodyParameter <IMicrosoftGraphChat> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgChat -InputObject <ITeamsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ChatType <String>] [-CreatedDateTime <DateTime>] [-Id <String>]
 [-InstalledApps <IMicrosoftGraphTeamsAppInstallation[]>] [-IsHiddenForAllMembers]
 [-LastMessagePreview <IMicrosoftGraphChatMessageInfo>] [-LastUpdatedDateTime <DateTime>]
 [-Members <IMicrosoftGraphConversationMember[]>] [-Messages <IMicrosoftGraphChatMessage[]>]
 [-OnlineMeetingInfo <IMicrosoftGraphTeamworkOnlineMeetingInfo>]
 [-PermissionGrants <IMicrosoftGraphResourceSpecificPermissionGrant[]>]
 [-PinnedMessages <IMicrosoftGraphPinnedChatMessageInfo[]>] [-Tabs <IMicrosoftGraphTeamsTab[]>]
 [-TenantId <String>] [-Topic <String>] [-Viewpoint <IMicrosoftGraphChatViewpoint>] [-WebUrl <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgChat -InputObject <ITeamsIdentity> -BodyParameter <IMicrosoftGraphChat>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of a chat object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Chat.ReadWrite,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | ChatSettings.ReadWrite.Chat, Chat.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
	topic = "Group chat title update"
}

Update-MgChat -ChatId $chatId -BodyParameter $params

```
This example shows how to use the Update-MgChat Cmdlet.


## PARAMETERS

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
chat
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphChat
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChatId
The unique identifier of chat

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

### -ChatType
chatType

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

### -CreatedDateTime
Date and time at which the chat was created.
Read-only.

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
Type: ITeamsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InstalledApps
A collection of all the apps in the chat.
Nullable.
To construct, see NOTES section for INSTALLEDAPPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsAppInstallation[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastUpdatedDateTime
Date and time at which the chat was renamed or the list of members was last changed.
Read-only.

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

### -Members
A collection of all the members in the chat.
Nullable.
To construct, see NOTES section for MEMBERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphConversationMember[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphChat
### Microsoft.Graph.PowerShell.Models.ITeamsIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphChat
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphChat>`: chat
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ChatType <String>]`: chatType
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
  - `[LastUpdatedDateTime <DateTime?>]`: Date and time at which the chat was renamed or the list of members was last changed.
Read-only.
  - `[Members <IMicrosoftGraphConversationMember- `[]`>]`: A collection of all the members in the chat.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: The display name of the user.
    - `[Roles <String- `[]`>]`: The roles for that user.
This property contains more qualifiers only when relevant - for example, if the member has owner privileges, the roles property contains owner as one of the values.
Similarly, if the member is an in-tenant guest, the roles property contains guest as one of the values.
A basic member shouldn't have any values specified in the roles property.
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
Populate the content with the original message context.Any contentType that is supported by the Bot Framework's Attachment object.application/vnd.microsoft.card.codesnippet: A code snippet.
application/vnd.microsoft.card.announcement: An announcement header.
      - `[ContentUrl <String>]`: The URL for the content of the attachment.
      - `[Id <String>]`: Read-only.
The unique ID of the attachment.
      - `[Name <String>]`: The name of the attachment.
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
Content type.
such as image/png, image/jpg.
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
          - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
          - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
          - `[ConversationIdentityType <String>]`: teamworkConversationIdentityType
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
    - `[JoinWebUrl <String>]`: The URL that users click to join or uniquely identify the meeting.
    - `[Organizer <IMicrosoftGraphTeamworkUserIdentity>]`: teamworkUserIdentity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
      - `[UserIdentityType <String>]`: teamworkUserIdentityType
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
    - `[TeamsApp <IMicrosoftGraphTeamsApp>]`: teamsApp
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

INSTALLEDAPPS `<IMicrosoftGraphTeamsAppInstallation- `[]`>`: A collection of all the apps in the chat.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ConsentedPermissionSet <IMicrosoftGraphTeamsAppPermissionSet>]`: teamsAppPermissionSet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ResourceSpecificPermissions <IMicrosoftGraphTeamsAppResourceSpecificPermission- `[]`>]`: A collection of resource-specific permissions.
      - `[PermissionType <String>]`: teamsAppResourceSpecificPermissionType
      - `[PermissionValue <String>]`: The name of the resource-specific permission.
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
      - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
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
This property contains more qualifiers only when relevant - for example, if the member has owner privileges, the roles property contains owner as one of the values.
Similarly, if the member is an in-tenant guest, the roles property contains guest as one of the values.
A basic member shouldn't have any values specified in the roles property.
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
Populate the content with the original message context.Any contentType that is supported by the Bot Framework's Attachment object.application/vnd.microsoft.card.codesnippet: A code snippet.
application/vnd.microsoft.card.announcement: An announcement header.
    - `[ContentUrl <String>]`: The URL for the content of the attachment.
    - `[Id <String>]`: Read-only.
The unique ID of the attachment.
    - `[Name <String>]`: The name of the attachment.
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
      - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[HostedContents <IMicrosoftGraphChatMessageHostedContent- `[]`>]`: Content in a message hosted by Microsoft Teams - for example, images or code snippets.
    - `[ContentBytes <Byte- `[]`>]`: Write only.
Bytes for the hosted content (such as images).
    - `[ContentType <String>]`: Write only.
Content type.
such as image/png, image/jpg.
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
        - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
        - `[ConversationIdentityType <String>]`: teamworkConversationIdentityType
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
  - `[JoinWebUrl <String>]`: The URL that users click to join or uniquely identify the meeting.
  - `[Organizer <IMicrosoftGraphTeamworkUserIdentity>]`: teamworkUserIdentity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
    - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
    - `[UserIdentityType <String>]`: teamworkUserIdentityType

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
Populate the content with the original message context.Any contentType that is supported by the Bot Framework's Attachment object.application/vnd.microsoft.card.codesnippet: A code snippet.
application/vnd.microsoft.card.announcement: An announcement header.
      - `[ContentUrl <String>]`: The URL for the content of the attachment.
      - `[Id <String>]`: Read-only.
The unique ID of the attachment.
      - `[Name <String>]`: The name of the attachment.
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
        - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[HostedContents <IMicrosoftGraphChatMessageHostedContent- `[]`>]`: Content in a message hosted by Microsoft Teams - for example, images or code snippets.
      - `[ContentBytes <Byte- `[]`>]`: Write only.
Bytes for the hosted content (such as images).
      - `[ContentType <String>]`: Write only.
Content type.
such as image/png, image/jpg.
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
          - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
          - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
          - `[ConversationIdentityType <String>]`: teamworkConversationIdentityType
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

VIEWPOINT `<IMicrosoftGraphChatViewpoint>`: chatViewpoint
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsHidden <Boolean?>]`: Indicates whether the chat is hidden for the current user.
  - `[LastMessageReadDateTime <DateTime?>]`: Represents the dateTime up until which the current user has read chatMessages in a specific chat.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.teams/update-mgchat](https://learn.microsoft.com/powershell/module/microsoft.graph.teams/update-mgchat)

[https://learn.microsoft.com/graph/api/chat-patch?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/chat-patch?view=graph-rest-1.0)























