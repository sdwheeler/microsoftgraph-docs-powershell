---
external help file: Microsoft.Graph.Beta.Applications-help.xml
Module Name: Microsoft.Graph.Beta.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/get-mgbetaapplicationdelta
schema: 2.0.0
ms.subservice: entra-applications
---

# Get-MgBetaApplicationDelta

## SYNOPSIS
Get newly created, updated, or deleted applications without having to perform a full read of the entire resource collection.
For more information, see Use delta query to track changes in Microsoft Graph data for details.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgApplicationDelta](/powershell/module/Microsoft.Graph.Applications/Get-MgApplicationDelta?view=graph-powershell-1.0)

## SYNTAX

```
Get-MgBetaApplicationDelta [-ExpandProperty <String[]>] [-Filter <String>] [-Property <String[]>]
 [-Search <String>] [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-PageSize <Int32>] [-All] [-CountVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
Get newly created, updated, or deleted applications without having to perform a full read of the entire resource collection.
For more information, see Use delta query to track changes in Microsoft Graph data for details.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Directory.Read.All, Directory.ReadWrite.All, Application.ReadWrite.All, Application.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Application.ReadWrite.OwnedBy, Directory.ReadWrite.All, Directory.Read.All, Application.ReadWrite.All, Application.Read.All,  |

## EXAMPLES
### Example

```powershell

Import-Module Microsoft.Graph.Beta.Applications

Get-MgBetaApplicationDelta

```
This example shows how to use the Get-MgBetaApplicationDelta Cmdlet.


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

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Expand

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

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphApplication
## NOTES

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/get-mgbetaapplicationdelta](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/get-mgbetaapplicationdelta)

[https://learn.microsoft.com/graph/api/application-delta?view=graph-rest-beta](https://learn.microsoft.com/graph/api/application-delta?view=graph-rest-beta)























