---
external help file: Microsoft.Graph.Beta.Mail-help.xml
Module Name: Microsoft.Graph.Beta.Mail
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/new-mgbetausermailfolderchildfoldermessagemention
schema: 2.0.0
---

# New-MgBetaUserMailFolderChildFolderMessageMention

## SYNOPSIS
Create new navigation property to mentions for users

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaUserMailFolderChildFolderMessageMention -MailFolderId <String> -MailFolderId1 <String>
 -MessageId <String> -UserId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Application <String>] [-ClientReference <String>] [-CreatedBy <IMicrosoftGraphEmailAddress>]
 [-CreatedDateTime <DateTime>] [-DeepLink <String>] [-Id <String>] [-MentionText <String>]
 [-Mentioned <IMicrosoftGraphEmailAddress>] [-ServerCreatedDateTime <DateTime>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaUserMailFolderChildFolderMessageMention -MailFolderId <String> -MailFolderId1 <String>
 -MessageId <String> -UserId <String> -BodyParameter <IMicrosoftGraphMention>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaUserMailFolderChildFolderMessageMention -InputObject <IMailIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Application <String>]
 [-ClientReference <String>] [-CreatedBy <IMicrosoftGraphEmailAddress>] [-CreatedDateTime <DateTime>]
 [-DeepLink <String>] [-Id <String>] [-MentionText <String>] [-Mentioned <IMicrosoftGraphEmailAddress>]
 [-ServerCreatedDateTime <DateTime>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaUserMailFolderChildFolderMessageMention -InputObject <IMailIdentity>
 -BodyParameter <IMicrosoftGraphMention> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to mentions for users

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

### -Application
The name of the application where the mention is created.
Optional.
Not used and defaulted as null for message.

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

### -BodyParameter
mention
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphMention
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ClientReference
A unique identifier that represents a parent of the resource instance.
Optional.
Not used and defaulted as null for message.

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
emailAddress
To construct, see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphEmailAddress
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
The date and time that the mention is created on the client.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeepLink
A deep web link to the context of the mention in the resource instance.
Optional.
Not used and defaulted as null for message.

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
Type: IMailIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
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
Parameter Sets: CreateExpanded, Create
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
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Mentioned
emailAddress
To construct, see NOTES section for MENTIONED properties and create a hash table.

```yaml
Type: IMicrosoftGraphEmailAddress
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MentionText
Optional.
Not used and defaulted as null for message.
To get the mentions in a message, see the bodyPreview property of the message instead.

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

### -MessageId
The unique identifier of message

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

### -ServerCreatedDateTime
The date and time that the mention is created on the server.
Optional.
Not used and defaulted as null for message.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, Create
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
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMention
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMention
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphMention>`: mention
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Application <String>]`: The name of the application where the mention is created.
Optional.
Not used and defaulted as null for message.
  - `[ClientReference <String>]`: A unique identifier that represents a parent of the resource instance.
Optional.
Not used and defaulted as null for message.
  - `[CreatedBy <IMicrosoftGraphEmailAddress>]`: emailAddress
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Address <String>]`: The email address of an entity instance.
    - `[Name <String>]`: The display name of an entity instance.
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

CREATEDBY `<IMicrosoftGraphEmailAddress>`: emailAddress
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Address <String>]`: The email address of an entity instance.
  - `[Name <String>]`: The display name of an entity instance.

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

MENTIONED `<IMicrosoftGraphEmailAddress>`: emailAddress
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Address <String>]`: The email address of an entity instance.
  - `[Name <String>]`: The display name of an entity instance.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/new-mgbetausermailfolderchildfoldermessagemention](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.mail/new-mgbetausermailfolderchildfoldermessagemention)
























