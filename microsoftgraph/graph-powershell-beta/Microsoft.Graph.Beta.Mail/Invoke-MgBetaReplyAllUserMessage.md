---
external help file: Microsoft.Graph.Beta.Mail-help.xml
Module Name: Microsoft.Graph.Beta.Mail
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/invoke-mgbetareplyallusermessage
schema: 2.0.0
ms.subservice: outlook
---

# Invoke-MgBetaReplyAllUserMessage

## SYNOPSIS
Reply to all recipients of a message using either JSON or MIME format.
When using JSON format:- Specify either a comment or the body property of the message parameter.
Specifying both will return an HTTP 400 Bad Request error.- If the original message specifies a recipient in the replyTo property, per Internet Message Format (RFC 2822), send the reply to the recipients in replyTo and not the recipient in the from property.
When using MIME format:- Provide the applicable Internet message headers and the MIME content, all encoded in base64 format in the request body.- Add any attachments and S/MIME properties to the MIME content.
This method saves the message in the Sent Items folder.
Alternatively, create a draft to reply-all to a message, and send it later.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Invoke-MgReplyAllUserMessage](/powershell/module/Microsoft.Graph.Mail/Invoke-MgReplyAllUserMessage?view=graph-powershell-1.0)

## SYNTAX

### ReplyExpanded1 (Default)
```
Invoke-MgBetaReplyAllUserMessage -MessageId <String> -UserId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Comment <String>] [-Message <IMicrosoftGraphMessage>]
 [-Headers <IDictionary>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Reply1
```
Invoke-MgBetaReplyAllUserMessage -MessageId <String> -UserId <String>
 -BodyParameter <IPathsKn6R94UsersUserIdMessagesMessageIdMicrosoftGraphReplyallPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ReplyViaIdentityExpanded1
```
Invoke-MgBetaReplyAllUserMessage -InputObject <IMailIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Comment <String>] [-Message <IMicrosoftGraphMessage>]
 [-Headers <IDictionary>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### ReplyViaIdentity1
```
Invoke-MgBetaReplyAllUserMessage -InputObject <IMailIdentity>
 -BodyParameter <IPathsKn6R94UsersUserIdMessagesMessageIdMicrosoftGraphReplyallPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Reply to all recipients of a message using either JSON or MIME format.
When using JSON format:- Specify either a comment or the body property of the message parameter.
Specifying both will return an HTTP 400 Bad Request error.- If the original message specifies a recipient in the replyTo property, per Internet Message Format (RFC 2822), send the reply to the recipients in replyTo and not the recipient in the from property.
When using MIME format:- Provide the applicable Internet message headers and the MIME content, all encoded in base64 format in the request body.- Add any attachments and S/MIME properties to the MIME content.
This method saves the message in the Sent Items folder.
Alternatively, create a draft to reply-all to a message, and send it later.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Mail.Send,  |
| Delegated (personal Microsoft account) | Mail.Send,  |
| Application | Mail.Send,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	message = @{
		attachments = @(
			@{
				"@odata.type" = "#microsoft.graph.fileAttachment"
				name = "guidelines.txt"
				contentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
			}
		)
	}
	comment = "Please take a look at the attached guidelines before you decide on the name."
}

# A UPN can also be used as -UserId.
Invoke-MgBetaReplyAllUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```
This example shows how to use the Invoke-MgBetaReplyAllUserMessage Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: ReplyExpanded1, ReplyViaIdentityExpanded1
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
Type: IPathsKn6R94UsersUserIdMessagesMessageIdMicrosoftGraphReplyallPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Reply1, ReplyViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Comment


```yaml
Type: String
Parameter Sets: ReplyExpanded1, ReplyViaIdentityExpanded1
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
Type: IMailIdentity
Parameter Sets: ReplyViaIdentityExpanded1, ReplyViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Message
message
To construct, see NOTES section for MESSAGE properties and create a hash table.

```yaml
Type: IMicrosoftGraphMessage
Parameter Sets: ReplyExpanded1, ReplyViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MessageId
The unique identifier of message

```yaml
Type: String
Parameter Sets: ReplyExpanded1, Reply1
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
Parameter Sets: ReplyExpanded1, Reply1
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

### Microsoft.Graph.Beta.PowerShell.Models.IMailIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IPathsKn6R94UsersUserIdMessagesMessageIdMicrosoftGraphReplyallPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsKn6R94UsersUserIdMessagesMessageIdMicrosoftGraphReplyallPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Comment <String>]`: 
  - `[Message <IMicrosoftGraphMessage>]`: message
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Categories <String- `[]`>]`: The categories associated with the item.
    - `[ChangeKey <String>]`: Identifies the version of the item.
Every time the item is changed, changeKey changes as well.
This allows Exchange to apply changes to the correct version of the object.
Read-only.
    - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Attachments <IMicrosoftGraphAttachment- `[]`>]`: The fileAttachment and itemAttachment attachments for the message.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ContentType <String>]`: The MIME type.
      - `[IsInline <Boolean?>]`: true if the attachment is an inline attachment; otherwise, false.
      - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[Name <String>]`: The display name of the attachment.
This does not need to be the actual file name.
      - `[Size <Int32?>]`: The length of the attachment in bytes.
    - `[BccRecipients <IMicrosoftGraphRecipient- `[]`>]`: The Bcc: recipients for the message.
      - `[EmailAddress <IMicrosoftGraphEmailAddress>]`: emailAddress
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Address <String>]`: The email address of an entity instance.
        - `[Name <String>]`: The display name of an entity instance.
    - `[Body <IMicrosoftGraphItemBody>]`: itemBody
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Content <String>]`: The content of the item.
      - `[ContentType <String>]`: bodyType
    - `[BodyPreview <String>]`: The first 255 characters of the message body.
It is in text format.
If the message contains instances of mention, this property would contain a concatenation of these mentions as well.
    - `[CcRecipients <IMicrosoftGraphRecipient- `[]`>]`: The Cc: recipients for the message.
    - `[ConversationId <String>]`: The ID of the conversation the email belongs to.
    - `[ConversationIndex <Byte- `[]`>]`: Indicates the position of the message within the conversation.
    - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the message.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Flag <IMicrosoftGraphFollowupFlag>]`: followupFlag
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CompletedDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
        - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
      - `[DueDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[FlagStatus <String>]`: followupFlagStatus
      - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[From <IMicrosoftGraphRecipient>]`: recipient
    - `[HasAttachments <Boolean?>]`: Indicates whether the message has attachments.
This property doesn't include inline attachments, so if a message contains only inline attachments, this property is false.
To verify the existence of inline attachments, parse the body property to look for a src attribute, such as <IMG src='cid:image001.jpg@01D26CD8.6C05F070'>.
    - `[Importance <String>]`: importance
    - `[InferenceClassification <String>]`: inferenceClassificationType
    - `[InternetMessageHeaders <IMicrosoftGraphInternetMessageHeader- `[]`>]`: A collection of message headers defined by RFC5322.
The set includes message headers indicating the network path taken by a message from the sender to the recipient.
It can also contain custom message headers that hold app data for the message. 
Returned only on applying a $select query option.
Read-only.
      - `[Name <String>]`: Represents the key in a key-value pair.
      - `[Value <String>]`: The value in a key-value pair.
    - `[InternetMessageId <String>]`: The message ID in the format specified by RFC5322.
Updatable only if isDraft is true.
    - `[IsDeliveryReceiptRequested <Boolean?>]`: Indicates whether a read receipt is requested for the message.
    - `[IsDraft <Boolean?>]`: Indicates whether the message is a draft.
A message is a draft if it hasn't been sent yet.
    - `[IsRead <Boolean?>]`: Indicates whether the message has been read.
    - `[IsReadReceiptRequested <Boolean?>]`: Indicates whether a read receipt is requested for the message.
    - `[Mentions <IMicrosoftGraphMention- `[]`>]`: A collection of mentions in the message, ordered by the createdDateTime from the newest to the oldest.
By default, a GET /messages does not return this property unless you apply $expand on the property.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Application <String>]`: The name of the application where the mention is created.
Optional.
Not used and defaulted as null for message.
      - `[ClientReference <String>]`: A unique identifier that represents a parent of the resource instance.
Optional.
Not used and defaulted as null for message.
      - `[CreatedBy <IMicrosoftGraphEmailAddress>]`: emailAddress
      - `[CreatedDateTime <DateTime?>]`: The date and time that the mention is created on the client.
      - `[DeepLink <String>]`: A deep web link to the context of the mention in the resource instance.
Optional.
Not used and defaulted as null for message.
      - `[MentionText <String>]`: Optional.
Not used and defaulted as null for message.
To get the mentions in a message, see the bodyPreview property of the message instead.
      - `[Mentioned <IMicrosoftGraphEmailAddress>]`: emailAddress
      - `[ServerCreatedDateTime <DateTime?>]`: The date and time that the mention is created on the server.
Optional.
Not used and defaulted as null for message.
    - `[MentionsPreview <IMicrosoftGraphMentionsPreview>]`: mentionsPreview
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsMentioned <Boolean?>]`: True if the signed-in user is mentioned in the parent resource instance.
Read-only.
Supports filter.
    - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the message.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Value <String- `[]`>]`: A collection of property values.
    - `[ParentFolderId <String>]`: The unique identifier for the message's parent mailFolder.
    - `[ReceivedDateTime <DateTime?>]`: The date and time the message was received. 
The date and time information uses ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[ReplyTo <IMicrosoftGraphRecipient- `[]`>]`: The email addresses to use when replying.
    - `[Sender <IMicrosoftGraphRecipient>]`: recipient
    - `[SentDateTime <DateTime?>]`: The date and time the message was sent. 
The date and time information uses ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>]`: The collection of single-value extended properties defined for the message.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Value <String>]`: A property value.
    - `[Subject <String>]`: The subject of the message.
    - `[ToRecipients <IMicrosoftGraphRecipient- `[]`>]`: The To: recipients for the message.
    - `[UniqueBody <IMicrosoftGraphItemBody>]`: itemBody
    - `[UnsubscribeData <String- `[]`>]`: The valid entries parsed from the List-Unsubscribe header. 
This is the data for the mail command in the List-Unsubscribe header if UnsubscribeEnabled property is true.
    - `[UnsubscribeEnabled <Boolean?>]`: Indicates whether the message is enabled for unsubscribe. 
Its valueTrue if the list-Unsubscribe header conforms to rfc-2369.
    - `[WebLink <String>]`: The URL to open the message in Outlook on the web.You can append an ispopout argument to the end of the URL to change how the message is displayed.
If ispopout is not present or if it is set to 1, then the message is shown in a popout window.
If ispopout is set to 0, the browser shows the message in the Outlook on the web review pane.The message opens in the browser if you are signed in to your mailbox via Outlook on the web.
You are prompted to sign in if you are not already signed in with the browser.This URL cannot be accessed from within an iFrame.

INPUTOBJECT `<IMailIdentity>`: Identity Parameter
  - `[AttachmentId <String>]`: The unique identifier of attachment
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[InferenceClassificationOverrideId <String>]`: The unique identifier of inferenceClassificationOverride
  - `[MailFolderId <String>]`: The unique identifier of mailFolder
  - `[MailFolderId1 <String>]`: The unique identifier of mailFolder
  - `[MailFolderOperationId <String>]`: The unique identifier of mailFolderOperation
  - `[MentionId <String>]`: The unique identifier of mention
  - `[MessageId <String>]`: The unique identifier of message
  - `[MessageRuleId <String>]`: The unique identifier of messageRule
  - `[UserConfigurationId <String>]`: The unique identifier of userConfiguration
  - `[UserId <String>]`: The unique identifier of user

MESSAGE `<IMicrosoftGraphMessage>`: message
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Categories <String- `[]`>]`: The categories associated with the item.
  - `[ChangeKey <String>]`: Identifies the version of the item.
Every time the item is changed, changeKey changes as well.
This allows Exchange to apply changes to the correct version of the object.
Read-only.
  - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Attachments <IMicrosoftGraphAttachment- `[]`>]`: The fileAttachment and itemAttachment attachments for the message.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ContentType <String>]`: The MIME type.
    - `[IsInline <Boolean?>]`: true if the attachment is an inline attachment; otherwise, false.
    - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Name <String>]`: The display name of the attachment.
This does not need to be the actual file name.
    - `[Size <Int32?>]`: The length of the attachment in bytes.
  - `[BccRecipients <IMicrosoftGraphRecipient- `[]`>]`: The Bcc: recipients for the message.
    - `[EmailAddress <IMicrosoftGraphEmailAddress>]`: emailAddress
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Address <String>]`: The email address of an entity instance.
      - `[Name <String>]`: The display name of an entity instance.
  - `[Body <IMicrosoftGraphItemBody>]`: itemBody
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Content <String>]`: The content of the item.
    - `[ContentType <String>]`: bodyType
  - `[BodyPreview <String>]`: The first 255 characters of the message body.
It is in text format.
If the message contains instances of mention, this property would contain a concatenation of these mentions as well.
  - `[CcRecipients <IMicrosoftGraphRecipient- `[]`>]`: The Cc: recipients for the message.
  - `[ConversationId <String>]`: The ID of the conversation the email belongs to.
  - `[ConversationIndex <Byte- `[]`>]`: Indicates the position of the message within the conversation.
  - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the message.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Flag <IMicrosoftGraphFollowupFlag>]`: followupFlag
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CompletedDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
      - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
    - `[DueDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[FlagStatus <String>]`: followupFlagStatus
    - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
  - `[From <IMicrosoftGraphRecipient>]`: recipient
  - `[HasAttachments <Boolean?>]`: Indicates whether the message has attachments.
This property doesn't include inline attachments, so if a message contains only inline attachments, this property is false.
To verify the existence of inline attachments, parse the body property to look for a src attribute, such as <IMG src='cid:image001.jpg@01D26CD8.6C05F070'>.
  - `[Importance <String>]`: importance
  - `[InferenceClassification <String>]`: inferenceClassificationType
  - `[InternetMessageHeaders <IMicrosoftGraphInternetMessageHeader- `[]`>]`: A collection of message headers defined by RFC5322.
The set includes message headers indicating the network path taken by a message from the sender to the recipient.
It can also contain custom message headers that hold app data for the message. 
Returned only on applying a $select query option.
Read-only.
    - `[Name <String>]`: Represents the key in a key-value pair.
    - `[Value <String>]`: The value in a key-value pair.
  - `[InternetMessageId <String>]`: The message ID in the format specified by RFC5322.
Updatable only if isDraft is true.
  - `[IsDeliveryReceiptRequested <Boolean?>]`: Indicates whether a read receipt is requested for the message.
  - `[IsDraft <Boolean?>]`: Indicates whether the message is a draft.
A message is a draft if it hasn't been sent yet.
  - `[IsRead <Boolean?>]`: Indicates whether the message has been read.
  - `[IsReadReceiptRequested <Boolean?>]`: Indicates whether a read receipt is requested for the message.
  - `[Mentions <IMicrosoftGraphMention- `[]`>]`: A collection of mentions in the message, ordered by the createdDateTime from the newest to the oldest.
By default, a GET /messages does not return this property unless you apply $expand on the property.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Application <String>]`: The name of the application where the mention is created.
Optional.
Not used and defaulted as null for message.
    - `[ClientReference <String>]`: A unique identifier that represents a parent of the resource instance.
Optional.
Not used and defaulted as null for message.
    - `[CreatedBy <IMicrosoftGraphEmailAddress>]`: emailAddress
    - `[CreatedDateTime <DateTime?>]`: The date and time that the mention is created on the client.
    - `[DeepLink <String>]`: A deep web link to the context of the mention in the resource instance.
Optional.
Not used and defaulted as null for message.
    - `[MentionText <String>]`: Optional.
Not used and defaulted as null for message.
To get the mentions in a message, see the bodyPreview property of the message instead.
    - `[Mentioned <IMicrosoftGraphEmailAddress>]`: emailAddress
    - `[ServerCreatedDateTime <DateTime?>]`: The date and time that the mention is created on the server.
Optional.
Not used and defaulted as null for message.
  - `[MentionsPreview <IMicrosoftGraphMentionsPreview>]`: mentionsPreview
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsMentioned <Boolean?>]`: True if the signed-in user is mentioned in the parent resource instance.
Read-only.
Supports filter.
  - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the message.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Value <String- `[]`>]`: A collection of property values.
  - `[ParentFolderId <String>]`: The unique identifier for the message's parent mailFolder.
  - `[ReceivedDateTime <DateTime?>]`: The date and time the message was received. 
The date and time information uses ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[ReplyTo <IMicrosoftGraphRecipient- `[]`>]`: The email addresses to use when replying.
  - `[Sender <IMicrosoftGraphRecipient>]`: recipient
  - `[SentDateTime <DateTime?>]`: The date and time the message was sent. 
The date and time information uses ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>]`: The collection of single-value extended properties defined for the message.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Value <String>]`: A property value.
  - `[Subject <String>]`: The subject of the message.
  - `[ToRecipients <IMicrosoftGraphRecipient- `[]`>]`: The To: recipients for the message.
  - `[UniqueBody <IMicrosoftGraphItemBody>]`: itemBody
  - `[UnsubscribeData <String- `[]`>]`: The valid entries parsed from the List-Unsubscribe header. 
This is the data for the mail command in the List-Unsubscribe header if UnsubscribeEnabled property is true.
  - `[UnsubscribeEnabled <Boolean?>]`: Indicates whether the message is enabled for unsubscribe. 
Its valueTrue if the list-Unsubscribe header conforms to rfc-2369.
  - `[WebLink <String>]`: The URL to open the message in Outlook on the web.You can append an ispopout argument to the end of the URL to change how the message is displayed.
If ispopout is not present or if it is set to 1, then the message is shown in a popout window.
If ispopout is set to 0, the browser shows the message in the Outlook on the web review pane.The message opens in the browser if you are signed in to your mailbox via Outlook on the web.
You are prompted to sign in if you are not already signed in with the browser.This URL cannot be accessed from within an iFrame.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/invoke-mgbetareplyallusermessage](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/invoke-mgbetareplyallusermessage)

[https://learn.microsoft.com/graph/api/message-replyall?view=graph-rest-beta](https://learn.microsoft.com/graph/api/message-replyall?view=graph-rest-beta)























