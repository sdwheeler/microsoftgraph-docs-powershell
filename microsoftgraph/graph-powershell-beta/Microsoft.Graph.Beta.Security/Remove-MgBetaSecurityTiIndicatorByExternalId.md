---
external help file: Microsoft.Graph.Beta.Security-help.xml
Module Name: Microsoft.Graph.Beta.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/remove-mgbetasecuritytiindicatorbyexternalid
schema: 2.0.0
ms.subservice: security
---

# Remove-MgBetaSecurityTiIndicatorByExternalId

## SYNOPSIS
Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.

## SYNTAX

### DeleteExpanded (Default)
```
Remove-MgBetaSecurityTiIndicatorByExternalId [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Value <String[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Delete
```
Remove-MgBetaSecurityTiIndicatorByExternalId
 -BodyParameter <IPaths1Jddi17SecurityTiindicatorsMicrosoftGraphDeletetiindicatorsbyexternalidPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | ThreatIndicators.ReadWrite.OwnedBy,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | ThreatIndicators.ReadWrite.OwnedBy,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	value = @(
	"externalId-value1"
"externalId-value2"
)
}

Remove-MgBetaSecurityTiIndicatorByExternalId -BodyParameter $params

```
This example shows how to use the Remove-MgBetaSecurityTiIndicatorByExternalId Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: DeleteExpanded
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
Type: IPaths1Jddi17SecurityTiindicatorsMicrosoftGraphDeletetiindicatorsbyexternalidPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Delete
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

### -Value


```yaml
Type: String[]
Parameter Sets: DeleteExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IPaths1Jddi17SecurityTiindicatorsMicrosoftGraphDeletetiindicatorsbyexternalidPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphResultInfo
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths1Jddi17SecurityTiindicatorsMicrosoftGraphDeletetiindicatorsbyexternalidPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Value <String- `[]`>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/remove-mgbetasecuritytiindicatorbyexternalid](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/remove-mgbetasecuritytiindicatorbyexternalid)

[https://learn.microsoft.com/graph/api/tiindicator-deletetiindicatorsbyexternalid?view=graph-rest-beta](https://learn.microsoft.com/graph/api/tiindicator-deletetiindicatorsbyexternalid?view=graph-rest-beta)























