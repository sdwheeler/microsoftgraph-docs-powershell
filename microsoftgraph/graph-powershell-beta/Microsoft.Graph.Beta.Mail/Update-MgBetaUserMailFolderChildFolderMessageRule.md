---
external help file: Microsoft.Graph.Beta.Mail-help.xml
Module Name: Microsoft.Graph.Beta.Mail
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/update-mgbetausermailfolderchildfoldermessagerule
schema: 2.0.0
---

# Update-MgBetaUserMailFolderChildFolderMessageRule

## SYNOPSIS
Update the navigation property messageRules in users

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgUserMailFolderChildFolderMessageRule](/powershell/module/Microsoft.Graph.Mail/Update-MgUserMailFolderChildFolderMessageRule?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaUserMailFolderChildFolderMessageRule -MailFolderId <String> -MailFolderId1 <String>
 -MessageRuleId <String> -UserId <String> [-ResponseHeadersVariable <String>]
 [-Actions <IMicrosoftGraphMessageRuleActions>] [-AdditionalProperties <Hashtable>]
 [-Conditions <IMicrosoftGraphMessageRulePredicates>] [-DisplayName <String>]
 [-Exceptions <IMicrosoftGraphMessageRulePredicates>] [-HasError] [-Id <String>] [-IsEnabled] [-IsReadOnly]
 [-Sequence <Int32>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Update
```
Update-MgBetaUserMailFolderChildFolderMessageRule -MailFolderId <String> -MailFolderId1 <String>
 -MessageRuleId <String> -UserId <String> -BodyParameter <IMicrosoftGraphMessageRule>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaUserMailFolderChildFolderMessageRule -InputObject <IMailIdentity>
 [-ResponseHeadersVariable <String>] [-Actions <IMicrosoftGraphMessageRuleActions>]
 [-AdditionalProperties <Hashtable>] [-Conditions <IMicrosoftGraphMessageRulePredicates>]
 [-DisplayName <String>] [-Exceptions <IMicrosoftGraphMessageRulePredicates>] [-HasError] [-Id <String>]
 [-IsEnabled] [-IsReadOnly] [-Sequence <Int32>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaUserMailFolderChildFolderMessageRule -InputObject <IMailIdentity>
 -BodyParameter <IMicrosoftGraphMessageRule> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property messageRules in users

## EXAMPLES

## PARAMETERS

### -Actions
messageRuleActions
To construct, see NOTES section for ACTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMessageRuleActions
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
messageRule
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphMessageRule
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Conditions
messageRulePredicates
To construct, see NOTES section for CONDITIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMessageRulePredicates
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
The display name of the rule.

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

### -Exceptions
messageRulePredicates
To construct, see NOTES section for EXCEPTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMessageRulePredicates
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HasError
Indicates whether the rule is in an error condition.
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

### -IsEnabled
Indicates whether the rule is enabled to be applied to messages.

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

### -IsReadOnly
Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.

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

### -MailFolderId1
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

### -MessageRuleId
The unique identifier of messageRule

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

### -Sequence
Indicates the order in which the rule is executed, among other rules.

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
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMessageRule
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMessageRule
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ACTIONS `<IMicrosoftGraphMessageRuleActions>`: messageRuleActions
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

BODYPARAMETER `<IMicrosoftGraphMessageRule>`: messageRule
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
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

CONDITIONS `<IMicrosoftGraphMessageRulePredicates>`: messageRulePredicates
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[BodyContains <String- `[]`>]`: Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.
  - `[BodyOrSubjectContains <String- `[]`>]`: Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.
  - `[Categories <String- `[]`>]`: Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.
  - `[FromAddresses <IMicrosoftGraphRecipient- `[]`>]`: Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.
    - `[EmailAddress <IMicrosoftGraphEmailAddress>]`: emailAddress
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Address <String>]`: The email address of an entity instance.
      - `[Name <String>]`: The display name of an entity instance.
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

EXCEPTIONS `<IMicrosoftGraphMessageRulePredicates>`: messageRulePredicates
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[BodyContains <String- `[]`>]`: Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.
  - `[BodyOrSubjectContains <String- `[]`>]`: Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.
  - `[Categories <String- `[]`>]`: Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.
  - `[FromAddresses <IMicrosoftGraphRecipient- `[]`>]`: Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.
    - `[EmailAddress <IMicrosoftGraphEmailAddress>]`: emailAddress
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Address <String>]`: The email address of an entity instance.
      - `[Name <String>]`: The display name of an entity instance.
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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/update-mgbetausermailfolderchildfoldermessagerule](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/update-mgbetausermailfolderchildfoldermessagerule)
























