---
external help file: Microsoft.Graph.Beta.Reports-help.xml
Module Name: Microsoft.Graph.Beta.Reports
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/update-mgbetareportslaazureadauthentication
schema: 2.0.0
---

# Update-MgBetaReportSlaAzureAdAuthentication

## SYNOPSIS
Update the navigation property azureADAuthentication in reports

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaReportSlaAzureAdAuthentication [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Attainments <IMicrosoftGraphServiceLevelAgreementAttainment[]>]
 [-Id <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Update
```
Update-MgBetaReportSlaAzureAdAuthentication -BodyParameter <IMicrosoftGraphAzureAdAuthentication>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property azureADAuthentication in reports

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

### -Attainments
SLA data for a Microsoft Entra tenant for a calendar month.
To construct, see NOTES section for ATTAINMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphServiceLevelAgreementAttainment[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
azureADAuthentication
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAzureAdAuthentication
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAzureAdAuthentication
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAzureAdAuthentication
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ATTAINMENTS `<IMicrosoftGraphServiceLevelAgreementAttainment- `[]`>`: SLA data for a Microsoft Entra tenant for a calendar month.
  - `[EndDate <DateTime?>]`: The end date for the calendar month for which SLA attainment is measured.
  - `[Score <Double?>]`: The level of SLA attainment achieved by the tenant for the calendar month identified, as described in Microsoft Entra SLA performance.
Values are truncated, not rounded, so the actual value is always equal to or higher than the displayed value.
Values are expressed as a percentage of availability for the tenant.
  - `[StartDate <DateTime?>]`: The start date for the calendar month for which SLA attainment is measured.

BODYPARAMETER `<IMicrosoftGraphAzureAdAuthentication>`: azureADAuthentication
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Attainments <IMicrosoftGraphServiceLevelAgreementAttainment- `[]`>]`: SLA data for a Microsoft Entra tenant for a calendar month.
    - `[EndDate <DateTime?>]`: The end date for the calendar month for which SLA attainment is measured.
    - `[Score <Double?>]`: The level of SLA attainment achieved by the tenant for the calendar month identified, as described in Microsoft Entra SLA performance.
Values are truncated, not rounded, so the actual value is always equal to or higher than the displayed value.
Values are expressed as a percentage of availability for the tenant.
    - `[StartDate <DateTime?>]`: The start date for the calendar month for which SLA attainment is measured.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/update-mgbetareportslaazureadauthentication](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/update-mgbetareportslaazureadauthentication)
























