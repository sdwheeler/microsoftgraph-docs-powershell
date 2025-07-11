---
external help file: Microsoft.Graph.Applications-help.xml
Module Name: Microsoft.Graph.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.applications/get-mgapplicationtokenissuancepolicybyref
schema: 2.0.0
ms.subservice: entra-applications
---

# Get-MgApplicationTokenIssuancePolicyByRef

## SYNOPSIS
List the tokenIssuancePolicy objects that are assigned to an application.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaApplicationTokenIssuancePolicyByRef](/powershell/module/Microsoft.Graph.Beta.Applications/Get-MgBetaApplicationTokenIssuancePolicyByRef?view=graph-powershell-beta)

## SYNTAX

```
Get-MgApplicationTokenIssuancePolicyByRef -ApplicationId <String> [-Filter <String>] [-Search <String>]
 [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-PageSize <Int32>] [-All] [-CountVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
List the tokenIssuancePolicy objects that are assigned to an application.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All, Application.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

### -All
List all pages.

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

### -ApplicationId
The unique identifier of application

```yaml
Type: String
Parameter Sets: (All)
Aliases: ObjectId

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CountVariable
Specifies a count of the total number of items in a collection.
By default, this variable will be set in the global scope.

```yaml
Type: String
Parameter Sets: (All)
Aliases: CV

Required: False
Position: Named
Default value: None
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

### -PageSize
Sets the page size of results.

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

### -Sort
Order items by property values

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: OrderBy

Required: False
Position: Named
Default value: None
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

### System.String
## NOTES

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.applications/get-mgapplicationtokenissuancepolicybyref](https://learn.microsoft.com/powershell/module/microsoft.graph.applications/get-mgapplicationtokenissuancepolicybyref)

[https://learn.microsoft.com/graph/api/application-list-tokenissuancepolicies?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/application-list-tokenissuancepolicies?view=graph-rest-1.0)
























