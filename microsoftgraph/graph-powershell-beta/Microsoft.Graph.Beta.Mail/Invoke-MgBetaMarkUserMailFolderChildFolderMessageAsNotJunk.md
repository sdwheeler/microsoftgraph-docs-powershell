---
external help file: Microsoft.Graph.Beta.Mail-help.xml
Module Name: Microsoft.Graph.Beta.Mail
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/invoke-mgbetamarkusermailfolderchildfoldermessageasnotjunk
schema: 2.0.0
ms.subservice: outlook
---

# Invoke-MgBetaMarkUserMailFolderChildFolderMessageAsNotJunk

## SYNOPSIS
Mark a message as not junk.
This API removes the sender from the list of blocked senders and moves the message to the Inbox folder, when moveToInbox is true.

## SYNTAX

### MarkExpanded (Default)
```
Invoke-MgBetaMarkUserMailFolderChildFolderMessageAsNotJunk -MailFolderId <String> -MailFolderId1 <String>
 -MessageId <String> -UserId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-MoveToInbox] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Mark
```
Invoke-MgBetaMarkUserMailFolderChildFolderMessageAsNotJunk -MailFolderId <String> -MailFolderId1 <String>
 -MessageId <String> -UserId <String>
 -BodyParameter <IPathsB8Bsb2UsersUserIdMailfoldersMailfolderIdChildfoldersMailfolderId1MessagesMessageIdMicrosoftGraphMarkasnotjunkPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### MarkViaIdentityExpanded
```
Invoke-MgBetaMarkUserMailFolderChildFolderMessageAsNotJunk -InputObject <IMailIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-MoveToInbox]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### MarkViaIdentity
```
Invoke-MgBetaMarkUserMailFolderChildFolderMessageAsNotJunk -InputObject <IMailIdentity>
 -BodyParameter <IPathsB8Bsb2UsersUserIdMailfoldersMailfolderIdChildfoldersMailfolderId1MessagesMessageIdMicrosoftGraphMarkasnotjunkPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Mark a message as not junk.
This API removes the sender from the list of blocked senders and moves the message to the Inbox folder, when moveToInbox is true.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: MarkExpanded, MarkViaIdentityExpanded
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
Type: IPathsB8Bsb2UsersUserIdMailfoldersMailfolderIdChildfoldersMailfolderId1MessagesMessageIdMicrosoftGraphMarkasnotjunkPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Mark, MarkViaIdentity
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
Parameter Sets: MarkViaIdentityExpanded, MarkViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MailFolderId
The unique identifier of mailFolder

```yaml
Type: String
Parameter Sets: MarkExpanded, Mark
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
Parameter Sets: MarkExpanded, Mark
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MessageId
The unique identifier of message

```yaml
Type: String
Parameter Sets: MarkExpanded, Mark
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MoveToInbox


```yaml
Type: SwitchParameter
Parameter Sets: MarkExpanded, MarkViaIdentityExpanded
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
Parameter Sets: MarkExpanded, Mark
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
### Microsoft.Graph.Beta.PowerShell.Models.IPathsB8Bsb2UsersUserIdMailfoldersMailfolderIdChildfoldersMailfolderId1MessagesMessageIdMicrosoftGraphMarkasnotjunkPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMessage
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsB8Bsb2UsersUserIdMailfoldersMailfolderIdChildfoldersMailfolderId1MessagesMessageIdMicrosoftGraphMarkasnotjunkPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[MoveToInbox <Boolean?>]`: 

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/invoke-mgbetamarkusermailfolderchildfoldermessageasnotjunk](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/invoke-mgbetamarkusermailfolderchildfoldermessageasnotjunk)

[https://learn.microsoft.com/graph/api/message-markasnotjunk?view=graph-rest-beta](https://learn.microsoft.com/graph/api/message-markasnotjunk?view=graph-rest-beta)
























