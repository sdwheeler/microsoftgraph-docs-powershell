---
external help file: Microsoft.Graph.Beta.Reports-help.xml
Module Name: Microsoft.Graph.Beta.Reports
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/get-mgbetareportsecurityattacksimulationtrainingusercoverage
schema: 2.0.0
ms.subservice: reports
---

# Get-MgBetaReportSecurityAttackSimulationTrainingUserCoverage

## SYNOPSIS
List training coverage for tenant users in attack simulation and training campaigns.
This function supports @odata.nextLink for pagination.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgReportSecurityAttackSimulationTrainingUserCoverage](/powershell/module/Microsoft.Graph.Reports/Get-MgReportSecurityAttackSimulationTrainingUserCoverage?view=graph-powershell-1.0)

## SYNTAX

```
Get-MgBetaReportSecurityAttackSimulationTrainingUserCoverage [-Count] [-Filter <String>] [-Search <String>]
 [-Skip <Int32>] [-Top <Int32>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
List training coverage for tenant users in attack simulation and training campaigns.
This function supports @odata.nextLink for pagination.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | AttackSimulation.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | AttackSimulation.Read.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Reports

Get-MgBetaReportSecurityAttackSimulationTrainingUserCoverage

```
This example shows how to use the Get-MgBetaReportSecurityAttackSimulationTrainingUserCoverage Cmdlet.


## PARAMETERS

### -Count
Include count of items

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

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: (All)
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

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Skip
Skip the first n items

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Top
Show only the first n items

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: Limit

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAttackSimulationTrainingUserCoverage
## NOTES

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/get-mgbetareportsecurityattacksimulationtrainingusercoverage](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/get-mgbetareportsecurityattacksimulationtrainingusercoverage)

[https://learn.microsoft.com/graph/api/securityreportsroot-getattacksimulationtrainingusercoverage?view=graph-rest-beta](https://learn.microsoft.com/graph/api/securityreportsroot-getattacksimulationtrainingusercoverage?view=graph-rest-beta)























