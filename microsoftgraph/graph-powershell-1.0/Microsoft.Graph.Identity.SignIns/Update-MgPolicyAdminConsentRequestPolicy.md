---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgpolicyadminconsentrequestpolicy
schema: 2.0.0
ms.subservice: entra-id-governance
---

# Update-MgPolicyAdminConsentRequestPolicy

## SYNOPSIS
Update the properties of an adminConsentRequestPolicy object.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaPolicyAdminConsentRequestPolicy](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/Update-MgBetaPolicyAdminConsentRequestPolicy?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgPolicyAdminConsentRequestPolicy [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Id <String>] [-IsEnabled] [-NotifyReviewers] [-RemindersEnabled]
 [-RequestDurationInDays <Int32>] [-Reviewers <IMicrosoftGraphAccessReviewReviewerScope[]>] [-Version <Int32>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgPolicyAdminConsentRequestPolicy -BodyParameter <IMicrosoftGraphAdminConsentRequestPolicy>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of an adminConsentRequestPolicy object.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
adminConsentRequestPolicy
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAdminConsentRequestPolicy
Parameter Sets: Update
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

### -Id
The unique identifier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsEnabled
Specifies whether the admin consent request feature is enabled or disabled.
Required.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NotifyReviewers
Specifies whether reviewers will receive notifications.
Required.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemindersEnabled
Specifies whether reviewers will receive reminder emails.
Required.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RequestDurationInDays
Specifies the duration the request is active before it automatically expires if no decision is applied.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
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

### -Reviewers
The list of reviewers for the admin consent.
Required.
To construct, see NOTES section for REVIEWERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewReviewerScope[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Version
Specifies the version of this policy.
When the policy is updated, this version is updated.
Read-only.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAdminConsentRequestPolicy
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAdminConsentRequestPolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphAdminConsentRequestPolicy>`: adminConsentRequestPolicy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[IsEnabled <Boolean?>]`: Specifies whether the admin consent request feature is enabled or disabled.
Required.
  - `[NotifyReviewers <Boolean?>]`: Specifies whether reviewers will receive notifications.
Required.
  - `[RemindersEnabled <Boolean?>]`: Specifies whether reviewers will receive reminder emails.
Required.
  - `[RequestDurationInDays <Int32?>]`: Specifies the duration the request is active before it automatically expires if no decision is applied.
  - `[Reviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: The list of reviewers for the admin consent.
Required.
    - `[Query <String>]`: The query specifying who will be the reviewer.
    - `[QueryRoot <String>]`: In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.
This property is only required if a relative query, for example, ./manager, is specified.
Possible value: decisions.
    - `[QueryType <String>]`: The type of query.
Examples include MicrosoftGraph and ARM.
  - `[Version <Int32?>]`: Specifies the version of this policy.
When the policy is updated, this version is updated.
Read-only.

REVIEWERS `<IMicrosoftGraphAccessReviewReviewerScope- `[]`>`: The list of reviewers for the admin consent.
Required.
  - `[Query <String>]`: The query specifying who will be the reviewer.
  - `[QueryRoot <String>]`: In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.
This property is only required if a relative query, for example, ./manager, is specified.
Possible value: decisions.
  - `[QueryType <String>]`: The type of query.
Examples include MicrosoftGraph and ARM.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgpolicyadminconsentrequestpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgpolicyadminconsentrequestpolicy)

[https://learn.microsoft.com/graph/api/adminconsentrequestpolicy-update?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/adminconsentrequestpolicy-update?view=graph-rest-1.0)
























