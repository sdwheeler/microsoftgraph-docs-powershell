---
external help file: Microsoft.Graph.Beta.Teams-help.xml
Module Name: Microsoft.Graph.Beta.Teams
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/send-mgbetateamworkactivitynotificationtorecipient
schema: 2.0.0
ms.subservice: teams
---

# Send-MgBetaTeamworkActivityNotificationToRecipient

## SYNOPSIS
Send activity feed notifications to multiple users in bulk.
For more information, see sending Teams activity notifications.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Send-MgTeamworkActivityNotificationToRecipient](/powershell/module/Microsoft.Graph.Teams/Send-MgTeamworkActivityNotificationToRecipient?view=graph-powershell-1.0)

## SYNTAX

### SendExpanded (Default)
```
Send-MgBetaTeamworkActivityNotificationToRecipient [-ResponseHeadersVariable <String>] [-ActivityType <String>]
 [-AdditionalProperties <Hashtable>] [-ChainId <Int64>] [-PreviewText <IMicrosoftGraphItemBody>]
 [-Recipients <IMicrosoftGraphTeamworkNotificationRecipient[]>] [-TeamsAppId <String>]
 [-TemplateParameters <IMicrosoftGraphKeyValuePair[]>] [-Topic <IMicrosoftGraphTeamworkActivityTopic>]
 [-Headers <IDictionary>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Send
```
Send-MgBetaTeamworkActivityNotificationToRecipient
 -BodyParameter <IPaths1T8Q21HTeamworkMicrosoftGraphSendactivitynotificationtorecipientsPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Send activity feed notifications to multiple users in bulk.
For more information, see sending Teams activity notifications.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | TeamsActivity.Send,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | TeamsActivity.Send.User, TeamsActivity.Send,  |

## EXAMPLES
### Example 1: Notify multiple users about pending finance approval requests

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	topic = @{
		source = "entityUrl"
		value = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}"
	}
	activityType = "pendingFinanceApprovalRequests"
	previewText = @{
		content = "Internal spending team has a pending finance approval requests"
	}
	recipients = @(
		@{
			"@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
			userId = "569363e2-4e49-4661-87f2-16f245c5d66a"
		}
		@{
			"@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
			userId = "ab88234e-0874-477c-9638-d144296ed04f"
		}
		@{
			"@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
			userId = "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
		}
	)
	templateParameters = @(
		@{
			name = "pendingRequestCount"
			value = "5"
		}
	)
}

Send-MgBetaTeamworkActivityNotificationToRecipient -BodyParameter $params

```
This example will notify multiple users about pending finance approval requests

### Example 2: Notify multiple users about an event using a custom topic

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	topic = @{
		source = "text"
		value = "Deployment Approvals Channel"
		webUrl = "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
	}
	activityType = "deploymentApprovalRequired"
	previewText = @{
		content = "New deployment requires your approval"
	}
	templateParameters = @(
		@{
			name = "deploymentId"
			value = "6788662"
		}
	)
	recipients = @(
		@{
			"@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
			userId = "569363e2-4e49-4661-87f2-16f245c5d66a"
		}
		@{
			"@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
			userId = "ab88234e-0874-477c-9638-d144296ed04f"
		}
		@{
			"@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
			userId = "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
		}
	)
}

Send-MgBetaTeamworkActivityNotificationToRecipient -BodyParameter $params

```
This example will notify multiple users about an event using a custom topic


## PARAMETERS

### -ActivityType


```yaml
Type: String
Parameter Sets: SendExpanded
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
Parameter Sets: SendExpanded
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
Type: IPaths1T8Q21HTeamworkMicrosoftGraphSendactivitynotificationtorecipientsPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Send
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChainId


```yaml
Type: Int64
Parameter Sets: SendExpanded
Aliases:

Required: False
Position: Named
Default value: 0
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

### -PreviewText
itemBody
To construct, see NOTES section for PREVIEWTEXT properties and create a hash table.

```yaml
Type: IMicrosoftGraphItemBody
Parameter Sets: SendExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Recipients


```yaml
Type: IMicrosoftGraphTeamworkNotificationRecipient[]
Parameter Sets: SendExpanded
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

### -TeamsAppId


```yaml
Type: String
Parameter Sets: SendExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TemplateParameters

To construct, see NOTES section for TEMPLATEPARAMETERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphKeyValuePair[]
Parameter Sets: SendExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Topic
teamworkActivityTopic
To construct, see NOTES section for TOPIC properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamworkActivityTopic
Parameter Sets: SendExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IPaths1T8Q21HTeamworkMicrosoftGraphSendactivitynotificationtorecipientsPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths1T8Q21HTeamworkMicrosoftGraphSendactivitynotificationtorecipientsPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ActivityType <String>]`: 
  - `[ChainId <Int64?>]`: 
  - `[PreviewText <IMicrosoftGraphItemBody>]`: itemBody
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Content <String>]`: The content of the item.
    - `[ContentType <String>]`: bodyType
  - `[Recipients <IMicrosoftGraphTeamworkNotificationRecipient- `[]`>]`: 
  - `[TeamsAppId <String>]`: 
  - `[TemplateParameters <IMicrosoftGraphKeyValuePair- `[]`>]`: 
    - `[Name <String>]`: Name for this key-value pair
    - `[Value <String>]`: Value for this key-value pair
  - `[Topic <IMicrosoftGraphTeamworkActivityTopic>]`: teamworkActivityTopic
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Source <String>]`: teamworkActivityTopicSource
    - `[Value <String>]`: The topic value.
If the value of the source property is entityUrl, this must be a Microsoft Graph URL.
If the value is text, this must be a plain text value.
    - `[WebUrl <String>]`: The link the user clicks when they select the notification.
Optional when source is entityUrl; required when source is text.

PREVIEWTEXT `<IMicrosoftGraphItemBody>`: itemBody
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Content <String>]`: The content of the item.
  - `[ContentType <String>]`: bodyType

TEMPLATEPARAMETERS `<IMicrosoftGraphKeyValuePair- `[]`>`: .
  - `[Name <String>]`: Name for this key-value pair
  - `[Value <String>]`: Value for this key-value pair

TOPIC `<IMicrosoftGraphTeamworkActivityTopic>`: teamworkActivityTopic
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Source <String>]`: teamworkActivityTopicSource
  - `[Value <String>]`: The topic value.
If the value of the source property is entityUrl, this must be a Microsoft Graph URL.
If the value is text, this must be a plain text value.
  - `[WebUrl <String>]`: The link the user clicks when they select the notification.
Optional when source is entityUrl; required when source is text.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/send-mgbetateamworkactivitynotificationtorecipient](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/send-mgbetateamworkactivitynotificationtorecipient)

[https://learn.microsoft.com/graph/api/teamwork-sendactivitynotificationtorecipients?view=graph-rest-beta](https://learn.microsoft.com/graph/api/teamwork-sendactivitynotificationtorecipients?view=graph-rest-beta)























