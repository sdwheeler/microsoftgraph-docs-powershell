---
external help file: Microsoft.Graph.Beta.Mail-help.xml
Module Name: Microsoft.Graph.Beta.Mail
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/update-mgbetausermailfolder
schema: 2.0.0
---

# Update-MgBetaUserMailFolder

## SYNOPSIS
Update the navigation property mailFolders in users

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgUserMailFolder](/powershell/module/Microsoft.Graph.Mail/Update-MgUserMailFolder?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaUserMailFolder -MailFolderId <String> -UserId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ChildFolderCount <Int32>] [-ChildFolders <IMicrosoftGraphMailFolder[]>]
 [-DisplayName <String>] [-Id <String>] [-IsHidden] [-MessageRules <IMicrosoftGraphMessageRule[]>]
 [-Messages <IMicrosoftGraphMessage[]>]
 [-MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>]
 [-Operations <IMicrosoftGraphMailFolderOperation[]>] [-ParentFolderId <String>]
 [-SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]
 [-TotalItemCount <Int32>] [-UnreadItemCount <Int32>]
 [-UserConfigurations <IMicrosoftGraphUserConfiguration[]>] [-WellKnownName <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaUserMailFolder -MailFolderId <String> -UserId <String> -BodyParameter <IMicrosoftGraphMailFolder>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaUserMailFolder -InputObject <IMailIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ChildFolderCount <Int32>] [-ChildFolders <IMicrosoftGraphMailFolder[]>]
 [-DisplayName <String>] [-Id <String>] [-IsHidden] [-MessageRules <IMicrosoftGraphMessageRule[]>]
 [-Messages <IMicrosoftGraphMessage[]>]
 [-MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>]
 [-Operations <IMicrosoftGraphMailFolderOperation[]>] [-ParentFolderId <String>]
 [-SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]
 [-TotalItemCount <Int32>] [-UnreadItemCount <Int32>]
 [-UserConfigurations <IMicrosoftGraphUserConfiguration[]>] [-WellKnownName <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaUserMailFolder -InputObject <IMailIdentity> -BodyParameter <IMicrosoftGraphMailFolder>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property mailFolders in users

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Mail.ReadWrite,  |
| Delegated (personal Microsoft account) | Mail.ReadWrite,  |
| Application | Mail.ReadWrite,  |

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	displayName = "displayName-value"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params
```
This example shows how to use the Update-MgBetaUserMailFolder Cmdlet.

To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


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
mailFolder
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphMailFolder
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChildFolderCount
The number of immediate child mailFolders in the current mailFolder.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -ChildFolders
The collection of child folders in the mailFolder.
To construct, see NOTES section for CHILDFOLDERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMailFolder[]
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

### -DisplayName
The mailFolder's display name.

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
Type: IMailIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsHidden
Indicates whether the mailFolder is hidden.
This property can be set only when creating the folder.
Find more information in Hidden mail folders.

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

### -MailFolderId
The unique identifier of mailFolder

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

### -MessageRules
The collection of rules that apply to the user's Inbox folder.
To construct, see NOTES section for MESSAGERULES properties and create a hash table.

```yaml
Type: IMicrosoftGraphMessageRule[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Messages
The collection of messages in the mailFolder.
To construct, see NOTES section for MESSAGES properties and create a hash table.

```yaml
Type: IMicrosoftGraphMessage[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MultiValueExtendedProperties
The collection of multi-value extended properties defined for the mailFolder.
Read-only.
Nullable.
To construct, see NOTES section for MULTIVALUEEXTENDEDPROPERTIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphMultiValueLegacyExtendedProperty[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Operations

To construct, see NOTES section for OPERATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMailFolderOperation[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ParentFolderId
The unique identifier for the mailFolder's parent mailFolder.

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

### -SingleValueExtendedProperties
The collection of single-value extended properties defined for the mailFolder.
Read-only.
Nullable.
To construct, see NOTES section for SINGLEVALUEEXTENDEDPROPERTIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSingleValueLegacyExtendedProperty[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TotalItemCount
The number of items in the mailFolder.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -UnreadItemCount
The number of items in the mailFolder marked as unread.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserConfigurations

To construct, see NOTES section for USERCONFIGURATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserConfiguration[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

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

### -WellKnownName
The well-known folder name for the folder.
The possible values are listed above.
This property is only set for default folders created by Outlook.
For other folders, this property is null.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMailIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMailFolder
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMailFolder
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphMailFolder>`: mailFolder
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ChildFolderCount <Int32?>]`: The number of immediate child mailFolders in the current mailFolder.
  - `[ChildFolders <IMicrosoftGraphMailFolder- `[]`>]`: The collection of child folders in the mailFolder.
  - `[DisplayName <String>]`: The mailFolder's display name.
  - `[IsHidden <Boolean?>]`: Indicates whether the mailFolder is hidden.
This property can be set only when creating the folder.
Find more information in Hidden mail folders.
  - `[MessageRules <IMicrosoftGraphMessageRule- `[]`>]`: The collection of rules that apply to the user's Inbox folder.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Actions <IMicrosoftGraphMessageRuleActions>]`: messageRuleActions
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AssignCategories <String- `[]`>]`: A list of categories to be assigned to a message.
      - `[CopyToFolder <String>]`: The ID of a folder that a message is to be copied to.
      - `[Delete <Boolean?>]`: Indicates whether a message should be moved to the Deleted Items folder.
      - `[ForwardAsAttachmentTo <IMicrosoftGraphRecipient- `[]`>]`: The email addresses of the recipients to which a message should be forwarded as an attachment.
        - `[EmailAddress <IMicrosoftGraphEmailAddress>]`: emailAddress
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Address <String>]`: The email address of an entity instance.
          - `[Name <String>]`: The display name of an entity instance.
      - `[ForwardTo <IMicrosoftGraphRecipient- `[]`>]`: The email addresses of the recipients to which a message should be forwarded.
      - `[MarkAsRead <Boolean?>]`: Indicates whether a message should be marked as read.
      - `[MarkImportance <String>]`: importance
      - `[MoveToFolder <String>]`: The ID of the folder that a message will be moved to.
      - `[PermanentDelete <Boolean?>]`: Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.
      - `[RedirectTo <IMicrosoftGraphRecipient- `[]`>]`: The email address to which a message should be redirected.
      - `[StopProcessingRules <Boolean?>]`: Indicates whether subsequent rules should be evaluated.
    - `[Conditions <IMicrosoftGraphMessageRulePredicates>]`: messageRulePredicates
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[BodyContains <String- `[]`>]`: Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.
      - `[BodyOrSubjectContains <String- `[]`>]`: Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.
      - `[Categories <String- `[]`>]`: Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.
      - `[FromAddresses <IMicrosoftGraphRecipient- `[]`>]`: Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.
      - `[HasAttachments <Boolean?>]`: Indicates whether an incoming message must have attachments in order for the condition or exception to apply.
      - `[HeaderContains <String- `[]`>]`: Represents the strings that appear in the headers of an incoming message in order for the condition or exception to apply.
      - `[Importance <String>]`: importance
      - `[IsApprovalRequest <Boolean?>]`: Indicates whether an incoming message must be an approval request in order for the condition or exception to apply.
      - `[IsAutomaticForward <Boolean?>]`: Indicates whether an incoming message must be automatically forwarded in order for the condition or exception to apply.
      - `[IsAutomaticReply <Boolean?>]`: Indicates whether an incoming message must be an auto reply in order for the condition or exception to apply.
      - `[IsEncrypted <Boolean?>]`: Indicates whether an incoming message must be encrypted in order for the condition or exception to apply.
      - `[IsMeetingRequest <Boolean?>]`: Indicates whether an incoming message must be a meeting request in order for the condition or exception to apply.
      - `[IsMeetingResponse <Boolean?>]`: Indicates whether an incoming message must be a meeting response in order for the condition or exception to apply.
      - `[IsNonDeliveryReport <Boolean?>]`: Indicates whether an incoming message must be a non-delivery report in order for the condition or exception to apply.
      - `[IsPermissionControlled <Boolean?>]`: Indicates whether an incoming message must be permission controlled (RMS-protected) in order for the condition or exception to apply.
      - `[IsReadReceipt <Boolean?>]`: Indicates whether an incoming message must be a read receipt in order for the condition or exception to apply.
      - `[IsSigned <Boolean?>]`: Indicates whether an incoming message must be S/MIME-signed in order for the condition or exception to apply.
      - `[IsVoicemail <Boolean?>]`: Indicates whether an incoming message must be a voice mail in order for the condition or exception to apply.
      - `[MessageActionFlag <String>]`: messageActionFlag
      - `[NotSentToMe <Boolean?>]`: Indicates whether the owner of the mailbox must not be a recipient of an incoming message in order for the condition or exception to apply.
      - `[RecipientContains <String- `[]`>]`: Represents the strings that appear in either the toRecipients or ccRecipients properties of an incoming message in order for the condition or exception to apply.
      - `[SenderContains <String- `[]`>]`: Represents the strings that appear in the from property of an incoming message in order for the condition or exception to apply.
      - `[Sensitivity <String>]`: sensitivity
      - `[SentCcMe <Boolean?>]`: Indicates whether the owner of the mailbox must be in the ccRecipients property of an incoming message in order for the condition or exception to apply.
      - `[SentOnlyToMe <Boolean?>]`: Indicates whether the owner of the mailbox must be the only recipient in an incoming message in order for the condition or exception to apply.
      - `[SentToAddresses <IMicrosoftGraphRecipient- `[]`>]`: Represents the email addresses that an incoming message must have been sent to in order for the condition or exception to apply.
      - `[SentToMe <Boolean?>]`: Indicates whether the owner of the mailbox must be in the toRecipients property of an incoming message in order for the condition or exception to apply.
      - `[SentToOrCcMe <Boolean?>]`: Indicates whether the owner of the mailbox must be in either a toRecipients or ccRecipients property of an incoming message in order for the condition or exception to apply.
      - `[SubjectContains <String- `[]`>]`: Represents the strings that appear in the subject of an incoming message in order for the condition or exception to apply.
      - `[WithinSizeRange <IMicrosoftGraphSizeRange>]`: sizeRange
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[MaximumSize <Int32?>]`: The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.
        - `[MinimumSize <Int32?>]`: The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.
    - `[DisplayName <String>]`: The display name of the rule.
    - `[Exceptions <IMicrosoftGraphMessageRulePredicates>]`: messageRulePredicates
    - `[HasError <Boolean?>]`: Indicates whether the rule is in an error condition.
Read-only.
    - `[IsEnabled <Boolean?>]`: Indicates whether the rule is enabled to be applied to messages.
    - `[IsReadOnly <Boolean?>]`: Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.
    - `[Sequence <Int32?>]`: Indicates the order in which the rule is executed, among other rules.
  - `[Messages <IMicrosoftGraphMessage- `[]`>]`: The collection of messages in the mailFolder.
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
  - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the mailFolder.
Read-only.
Nullable.
  - `[Operations <IMicrosoftGraphMailFolderOperation- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ResourceLocation <String>]`: 
    - `[Status <String>]`: mailFolderOperationStatus
  - `[ParentFolderId <String>]`: The unique identifier for the mailFolder's parent mailFolder.
  - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>]`: The collection of single-value extended properties defined for the mailFolder.
Read-only.
Nullable.
  - `[TotalItemCount <Int32?>]`: The number of items in the mailFolder.
  - `[UnreadItemCount <Int32?>]`: The number of items in the mailFolder marked as unread.
  - `[UserConfigurations <IMicrosoftGraphUserConfiguration- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[BinaryData <Byte- `[]`>]`: 
  - `[WellKnownName <String>]`: The well-known folder name for the folder.
The possible values are listed above.
This property is only set for default folders created by Outlook.
For other folders, this property is null.

CHILDFOLDERS `<IMicrosoftGraphMailFolder- `[]`>`: The collection of child folders in the mailFolder.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ChildFolderCount <Int32?>]`: The number of immediate child mailFolders in the current mailFolder.
  - `[ChildFolders <IMicrosoftGraphMailFolder- `[]`>]`: The collection of child folders in the mailFolder.
  - `[DisplayName <String>]`: The mailFolder's display name.
  - `[IsHidden <Boolean?>]`: Indicates whether the mailFolder is hidden.
This property can be set only when creating the folder.
Find more information in Hidden mail folders.
  - `[MessageRules <IMicrosoftGraphMessageRule- `[]`>]`: The collection of rules that apply to the user's Inbox folder.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Actions <IMicrosoftGraphMessageRuleActions>]`: messageRuleActions
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AssignCategories <String- `[]`>]`: A list of categories to be assigned to a message.
      - `[CopyToFolder <String>]`: The ID of a folder that a message is to be copied to.
      - `[Delete <Boolean?>]`: Indicates whether a message should be moved to the Deleted Items folder.
      - `[ForwardAsAttachmentTo <IMicrosoftGraphRecipient- `[]`>]`: The email addresses of the recipients to which a message should be forwarded as an attachment.
        - `[EmailAddress <IMicrosoftGraphEmailAddress>]`: emailAddress
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Address <String>]`: The email address of an entity instance.
          - `[Name <String>]`: The display name of an entity instance.
      - `[ForwardTo <IMicrosoftGraphRecipient- `[]`>]`: The email addresses of the recipients to which a message should be forwarded.
      - `[MarkAsRead <Boolean?>]`: Indicates whether a message should be marked as read.
      - `[MarkImportance <String>]`: importance
      - `[MoveToFolder <String>]`: The ID of the folder that a message will be moved to.
      - `[PermanentDelete <Boolean?>]`: Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.
      - `[RedirectTo <IMicrosoftGraphRecipient- `[]`>]`: The email address to which a message should be redirected.
      - `[StopProcessingRules <Boolean?>]`: Indicates whether subsequent rules should be evaluated.
    - `[Conditions <IMicrosoftGraphMessageRulePredicates>]`: messageRulePredicates
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[BodyContains <String- `[]`>]`: Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.
      - `[BodyOrSubjectContains <String- `[]`>]`: Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.
      - `[Categories <String- `[]`>]`: Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.
      - `[FromAddresses <IMicrosoftGraphRecipient- `[]`>]`: Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.
      - `[HasAttachments <Boolean?>]`: Indicates whether an incoming message must have attachments in order for the condition or exception to apply.
      - `[HeaderContains <String- `[]`>]`: Represents the strings that appear in the headers of an incoming message in order for the condition or exception to apply.
      - `[Importance <String>]`: importance
      - `[IsApprovalRequest <Boolean?>]`: Indicates whether an incoming message must be an approval request in order for the condition or exception to apply.
      - `[IsAutomaticForward <Boolean?>]`: Indicates whether an incoming message must be automatically forwarded in order for the condition or exception to apply.
      - `[IsAutomaticReply <Boolean?>]`: Indicates whether an incoming message must be an auto reply in order for the condition or exception to apply.
      - `[IsEncrypted <Boolean?>]`: Indicates whether an incoming message must be encrypted in order for the condition or exception to apply.
      - `[IsMeetingRequest <Boolean?>]`: Indicates whether an incoming message must be a meeting request in order for the condition or exception to apply.
      - `[IsMeetingResponse <Boolean?>]`: Indicates whether an incoming message must be a meeting response in order for the condition or exception to apply.
      - `[IsNonDeliveryReport <Boolean?>]`: Indicates whether an incoming message must be a non-delivery report in order for the condition or exception to apply.
      - `[IsPermissionControlled <Boolean?>]`: Indicates whether an incoming message must be permission controlled (RMS-protected) in order for the condition or exception to apply.
      - `[IsReadReceipt <Boolean?>]`: Indicates whether an incoming message must be a read receipt in order for the condition or exception to apply.
      - `[IsSigned <Boolean?>]`: Indicates whether an incoming message must be S/MIME-signed in order for the condition or exception to apply.
      - `[IsVoicemail <Boolean?>]`: Indicates whether an incoming message must be a voice mail in order for the condition or exception to apply.
      - `[MessageActionFlag <String>]`: messageActionFlag
      - `[NotSentToMe <Boolean?>]`: Indicates whether the owner of the mailbox must not be a recipient of an incoming message in order for the condition or exception to apply.
      - `[RecipientContains <String- `[]`>]`: Represents the strings that appear in either the toRecipients or ccRecipients properties of an incoming message in order for the condition or exception to apply.
      - `[SenderContains <String- `[]`>]`: Represents the strings that appear in the from property of an incoming message in order for the condition or exception to apply.
      - `[Sensitivity <String>]`: sensitivity
      - `[SentCcMe <Boolean?>]`: Indicates whether the owner of the mailbox must be in the ccRecipients property of an incoming message in order for the condition or exception to apply.
      - `[SentOnlyToMe <Boolean?>]`: Indicates whether the owner of the mailbox must be the only recipient in an incoming message in order for the condition or exception to apply.
      - `[SentToAddresses <IMicrosoftGraphRecipient- `[]`>]`: Represents the email addresses that an incoming message must have been sent to in order for the condition or exception to apply.
      - `[SentToMe <Boolean?>]`: Indicates whether the owner of the mailbox must be in the toRecipients property of an incoming message in order for the condition or exception to apply.
      - `[SentToOrCcMe <Boolean?>]`: Indicates whether the owner of the mailbox must be in either a toRecipients or ccRecipients property of an incoming message in order for the condition or exception to apply.
      - `[SubjectContains <String- `[]`>]`: Represents the strings that appear in the subject of an incoming message in order for the condition or exception to apply.
      - `[WithinSizeRange <IMicrosoftGraphSizeRange>]`: sizeRange
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[MaximumSize <Int32?>]`: The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.
        - `[MinimumSize <Int32?>]`: The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.
    - `[DisplayName <String>]`: The display name of the rule.
    - `[Exceptions <IMicrosoftGraphMessageRulePredicates>]`: messageRulePredicates
    - `[HasError <Boolean?>]`: Indicates whether the rule is in an error condition.
Read-only.
    - `[IsEnabled <Boolean?>]`: Indicates whether the rule is enabled to be applied to messages.
    - `[IsReadOnly <Boolean?>]`: Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.
    - `[Sequence <Int32?>]`: Indicates the order in which the rule is executed, among other rules.
  - `[Messages <IMicrosoftGraphMessage- `[]`>]`: The collection of messages in the mailFolder.
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
  - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the mailFolder.
Read-only.
Nullable.
  - `[Operations <IMicrosoftGraphMailFolderOperation- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ResourceLocation <String>]`: 
    - `[Status <String>]`: mailFolderOperationStatus
  - `[ParentFolderId <String>]`: The unique identifier for the mailFolder's parent mailFolder.
  - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>]`: The collection of single-value extended properties defined for the mailFolder.
Read-only.
Nullable.
  - `[TotalItemCount <Int32?>]`: The number of items in the mailFolder.
  - `[UnreadItemCount <Int32?>]`: The number of items in the mailFolder marked as unread.
  - `[UserConfigurations <IMicrosoftGraphUserConfiguration- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[BinaryData <Byte- `[]`>]`: 
  - `[WellKnownName <String>]`: The well-known folder name for the folder.
The possible values are listed above.
This property is only set for default folders created by Outlook.
For other folders, this property is null.

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

MESSAGERULES `<IMicrosoftGraphMessageRule- `[]`>`: The collection of rules that apply to the user's Inbox folder.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Actions <IMicrosoftGraphMessageRuleActions>]`: messageRuleActions
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AssignCategories <String- `[]`>]`: A list of categories to be assigned to a message.
    - `[CopyToFolder <String>]`: The ID of a folder that a message is to be copied to.
    - `[Delete <Boolean?>]`: Indicates whether a message should be moved to the Deleted Items folder.
    - `[ForwardAsAttachmentTo <IMicrosoftGraphRecipient- `[]`>]`: The email addresses of the recipients to which a message should be forwarded as an attachment.
      - `[EmailAddress <IMicrosoftGraphEmailAddress>]`: emailAddress
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Address <String>]`: The email address of an entity instance.
        - `[Name <String>]`: The display name of an entity instance.
    - `[ForwardTo <IMicrosoftGraphRecipient- `[]`>]`: The email addresses of the recipients to which a message should be forwarded.
    - `[MarkAsRead <Boolean?>]`: Indicates whether a message should be marked as read.
    - `[MarkImportance <String>]`: importance
    - `[MoveToFolder <String>]`: The ID of the folder that a message will be moved to.
    - `[PermanentDelete <Boolean?>]`: Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.
    - `[RedirectTo <IMicrosoftGraphRecipient- `[]`>]`: The email address to which a message should be redirected.
    - `[StopProcessingRules <Boolean?>]`: Indicates whether subsequent rules should be evaluated.
  - `[Conditions <IMicrosoftGraphMessageRulePredicates>]`: messageRulePredicates
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[BodyContains <String- `[]`>]`: Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.
    - `[BodyOrSubjectContains <String- `[]`>]`: Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.
    - `[Categories <String- `[]`>]`: Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.
    - `[FromAddresses <IMicrosoftGraphRecipient- `[]`>]`: Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.
    - `[HasAttachments <Boolean?>]`: Indicates whether an incoming message must have attachments in order for the condition or exception to apply.
    - `[HeaderContains <String- `[]`>]`: Represents the strings that appear in the headers of an incoming message in order for the condition or exception to apply.
    - `[Importance <String>]`: importance
    - `[IsApprovalRequest <Boolean?>]`: Indicates whether an incoming message must be an approval request in order for the condition or exception to apply.
    - `[IsAutomaticForward <Boolean?>]`: Indicates whether an incoming message must be automatically forwarded in order for the condition or exception to apply.
    - `[IsAutomaticReply <Boolean?>]`: Indicates whether an incoming message must be an auto reply in order for the condition or exception to apply.
    - `[IsEncrypted <Boolean?>]`: Indicates whether an incoming message must be encrypted in order for the condition or exception to apply.
    - `[IsMeetingRequest <Boolean?>]`: Indicates whether an incoming message must be a meeting request in order for the condition or exception to apply.
    - `[IsMeetingResponse <Boolean?>]`: Indicates whether an incoming message must be a meeting response in order for the condition or exception to apply.
    - `[IsNonDeliveryReport <Boolean?>]`: Indicates whether an incoming message must be a non-delivery report in order for the condition or exception to apply.
    - `[IsPermissionControlled <Boolean?>]`: Indicates whether an incoming message must be permission controlled (RMS-protected) in order for the condition or exception to apply.
    - `[IsReadReceipt <Boolean?>]`: Indicates whether an incoming message must be a read receipt in order for the condition or exception to apply.
    - `[IsSigned <Boolean?>]`: Indicates whether an incoming message must be S/MIME-signed in order for the condition or exception to apply.
    - `[IsVoicemail <Boolean?>]`: Indicates whether an incoming message must be a voice mail in order for the condition or exception to apply.
    - `[MessageActionFlag <String>]`: messageActionFlag
    - `[NotSentToMe <Boolean?>]`: Indicates whether the owner of the mailbox must not be a recipient of an incoming message in order for the condition or exception to apply.
    - `[RecipientContains <String- `[]`>]`: Represents the strings that appear in either the toRecipients or ccRecipients properties of an incoming message in order for the condition or exception to apply.
    - `[SenderContains <String- `[]`>]`: Represents the strings that appear in the from property of an incoming message in order for the condition or exception to apply.
    - `[Sensitivity <String>]`: sensitivity
    - `[SentCcMe <Boolean?>]`: Indicates whether the owner of the mailbox must be in the ccRecipients property of an incoming message in order for the condition or exception to apply.
    - `[SentOnlyToMe <Boolean?>]`: Indicates whether the owner of the mailbox must be the only recipient in an incoming message in order for the condition or exception to apply.
    - `[SentToAddresses <IMicrosoftGraphRecipient- `[]`>]`: Represents the email addresses that an incoming message must have been sent to in order for the condition or exception to apply.
    - `[SentToMe <Boolean?>]`: Indicates whether the owner of the mailbox must be in the toRecipients property of an incoming message in order for the condition or exception to apply.
    - `[SentToOrCcMe <Boolean?>]`: Indicates whether the owner of the mailbox must be in either a toRecipients or ccRecipients property of an incoming message in order for the condition or exception to apply.
    - `[SubjectContains <String- `[]`>]`: Represents the strings that appear in the subject of an incoming message in order for the condition or exception to apply.
    - `[WithinSizeRange <IMicrosoftGraphSizeRange>]`: sizeRange
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[MaximumSize <Int32?>]`: The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.
      - `[MinimumSize <Int32?>]`: The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.
  - `[DisplayName <String>]`: The display name of the rule.
  - `[Exceptions <IMicrosoftGraphMessageRulePredicates>]`: messageRulePredicates
  - `[HasError <Boolean?>]`: Indicates whether the rule is in an error condition.
Read-only.
  - `[IsEnabled <Boolean?>]`: Indicates whether the rule is enabled to be applied to messages.
  - `[IsReadOnly <Boolean?>]`: Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.
  - `[Sequence <Int32?>]`: Indicates the order in which the rule is executed, among other rules.

MESSAGES `<IMicrosoftGraphMessage- `[]`>`: The collection of messages in the mailFolder.
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

MULTIVALUEEXTENDEDPROPERTIES `<IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>`: The collection of multi-value extended properties defined for the mailFolder.
Read-only.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Value <String- `[]`>]`: A collection of property values.

OPERATIONS `<IMicrosoftGraphMailFolderOperation- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ResourceLocation <String>]`: 
  - `[Status <String>]`: mailFolderOperationStatus

SINGLEVALUEEXTENDEDPROPERTIES `<IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>`: The collection of single-value extended properties defined for the mailFolder.
Read-only.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Value <String>]`: A property value.

USERCONFIGURATIONS `<IMicrosoftGraphUserConfiguration- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[BinaryData <Byte- `[]`>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/update-mgbetausermailfolder](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/update-mgbetausermailfolder)























