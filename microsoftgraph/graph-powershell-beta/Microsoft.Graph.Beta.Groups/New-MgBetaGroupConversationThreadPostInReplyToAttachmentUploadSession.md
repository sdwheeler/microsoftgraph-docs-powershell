---
external help file: Microsoft.Graph.Beta.Groups-help.xml
Module Name: Microsoft.Graph.Beta.Groups
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.groups/new-mgbetagroupconversationthreadpostinreplytoattachmentuploadsession
schema: 2.0.0
ms.subservice: outlook
---

# New-MgBetaGroupConversationThreadPostInReplyToAttachmentUploadSession

## SYNOPSIS
Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to an Outlook item.
The item can be a message or event.
Use this approach to attach a file if the file size is between 3 MB and 150 MB.
To attach a file that's smaller than 3 MB, do a POST operation on the attachments navigation property of the Outlook item; see how to do this for a message or for an event.
As part of the response, this action returns an upload URL that you can use in subsequent sequential PUT queries.
Request headers for each PUT operation let you specify the exact range of bytes to be uploaded.
This allows transfer to be resumed, in case the network connection is dropped during upload.
The following are the steps to attach a file to an Outlook item using an upload session: See attach large files to Outlook messages or events for an example.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgGroupConversationThreadPostInReplyToAttachmentUploadSession](/powershell/module/Microsoft.Graph.Groups/New-MgGroupConversationThreadPostInReplyToAttachmentUploadSession?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaGroupConversationThreadPostInReplyToAttachmentUploadSession -ConversationId <String>
 -ConversationThreadId <String> -GroupId <String> -PostId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AttachmentItem <IMicrosoftGraphAttachmentItem>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaGroupConversationThreadPostInReplyToAttachmentUploadSession -ConversationId <String>
 -ConversationThreadId <String> -GroupId <String> -PostId <String>
 -BodyParameter <IPaths64Ja8VGroupsGroupIdConversationsConversationIdThreadsConversationthreadIdPostsPostIdInreplytoAttachmentsMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaGroupConversationThreadPostInReplyToAttachmentUploadSession -InputObject <IGroupsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AttachmentItem <IMicrosoftGraphAttachmentItem>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaGroupConversationThreadPostInReplyToAttachmentUploadSession -InputObject <IGroupsIdentity>
 -BodyParameter <IPaths64Ja8VGroupsGroupIdConversationsConversationIdThreadsConversationthreadIdPostsPostIdInreplytoAttachmentsMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to an Outlook item.
The item can be a message or event.
Use this approach to attach a file if the file size is between 3 MB and 150 MB.
To attach a file that's smaller than 3 MB, do a POST operation on the attachments navigation property of the Outlook item; see how to do this for a message or for an event.
As part of the response, this action returns an upload URL that you can use in subsequent sequential PUT queries.
Request headers for each PUT operation let you specify the exact range of bytes to be uploaded.
This allows transfer to be resumed, in case the network connection is dropped during upload.
The following are the steps to attach a file to an Outlook item using an upload session: See attach large files to Outlook messages or events for an example.

## EXAMPLES

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

### -AttachmentItem
attachmentItem
To construct, see NOTES section for ATTACHMENTITEM properties and create a hash table.

```yaml
Type: IMicrosoftGraphAttachmentItem
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Type: IPaths64Ja8VGroupsGroupIdConversationsConversationIdThreadsConversationthreadIdPostsPostIdInreplytoAttachmentsMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema
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

### -ConversationId
The unique identifier of conversation

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

### -ConversationThreadId
The unique identifier of conversationThread

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

### -GroupId
The unique identifier of group

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
Type: IGroupsIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PostId
The unique identifier of post

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

### Microsoft.Graph.Beta.PowerShell.Models.IGroupsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IPaths64Ja8VGroupsGroupIdConversationsConversationIdThreadsConversationthreadIdPostsPostIdInreplytoAttachmentsMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUploadSession
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ATTACHMENTITEM `<IMicrosoftGraphAttachmentItem>`: attachmentItem
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AttachmentType <String>]`: attachmentType
  - `[ContentId <String>]`: The CID or Content-Id of the attachment for referencing in case of in-line attachments using <img src='cid:contentId'> tag in HTML messages.
Optional.
  - `[ContentType <String>]`: The nature of the data in the attachment.
Optional.
  - `[IsInline <Boolean?>]`: true if the attachment is an inline attachment; otherwise, false.
Optional.
  - `[Name <String>]`: The display name of the attachment.
This can be a descriptive string and doesn't have to be the actual file name.
Required.
  - `[Size <Int64?>]`: The length of the attachment in bytes.
Required.

BODYPARAMETER `<IPaths64Ja8VGroupsGroupIdConversationsConversationIdThreadsConversationthreadIdPostsPostIdInreplytoAttachmentsMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AttachmentItem <IMicrosoftGraphAttachmentItem>]`: attachmentItem
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AttachmentType <String>]`: attachmentType
    - `[ContentId <String>]`: The CID or Content-Id of the attachment for referencing in case of in-line attachments using <img src='cid:contentId'> tag in HTML messages.
Optional.
    - `[ContentType <String>]`: The nature of the data in the attachment.
Optional.
    - `[IsInline <Boolean?>]`: true if the attachment is an inline attachment; otherwise, false.
Optional.
    - `[Name <String>]`: The display name of the attachment.
This can be a descriptive string and doesn't have to be the actual file name.
Required.
    - `[Size <Int64?>]`: The length of the attachment in bytes.
Required.

INPUTOBJECT `<IGroupsIdentity>`: Identity Parameter
  - `[AttachmentId <String>]`: The unique identifier of attachment
  - `[ConversationId <String>]`: The unique identifier of conversation
  - `[ConversationThreadId <String>]`: The unique identifier of conversationThread
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[DirectorySettingId <String>]`: The unique identifier of directorySetting
  - `[EndDateTime <String>]`: Usage: endDateTime='{endDateTime}'
  - `[EndpointId <String>]`: The unique identifier of endpoint
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[GroupId <String>]`: The unique identifier of group
  - `[GroupLifecyclePolicyId <String>]`: The unique identifier of groupLifecyclePolicy
  - `[Interval <String>]`: Usage: interval='{interval}'
  - `[ListId <String>]`: Usage: listId='{listId}'
  - `[MentionId <String>]`: The unique identifier of mention
  - `[ModelName <String>]`: Usage: modelName='{modelName}'
  - `[Path <String>]`: Usage: path='{path}'
  - `[PostId <String>]`: The unique identifier of post
  - `[ProfilePhotoId <String>]`: The unique identifier of profilePhoto
  - `[ResourceSpecificPermissionGrantId <String>]`: The unique identifier of resourceSpecificPermissionGrant
  - `[SiteId <String>]`: The unique identifier of site
  - `[StartDateTime <String>]`: Usage: startDateTime='{startDateTime}'
  - `[UniqueName <String>]`: Alternate key of group
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.groups/new-mgbetagroupconversationthreadpostinreplytoattachmentuploadsession](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.groups/new-mgbetagroupconversationthreadpostinreplytoattachmentuploadsession)

[https://learn.microsoft.com/graph/api/attachment-createuploadsession?view=graph-rest-beta](https://learn.microsoft.com/graph/api/attachment-createuploadsession?view=graph-rest-beta)
























