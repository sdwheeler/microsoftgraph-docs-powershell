---
external help file: Microsoft.Graph.Beta.Applications-help.xml
Module Name: Microsoft.Graph.Beta.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/get-mgbetaserviceprincipalownerbyref
schema: 2.0.0
---

# Get-MgBetaServicePrincipalOwnerByRef

## SYNOPSIS
Directory objects that are owners of this servicePrincipal.
The owners are a set of nonadmin users or servicePrincipals who are allowed to modify this object.
Supports $expand and $filter (/$count eq 0, /$count ne 0, /$count eq 1, /$count ne 1).

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgServicePrincipalOwnerByRef](/powershell/module/Microsoft.Graph.Applications/Get-MgServicePrincipalOwnerByRef?view=graph-powershell-1.0)

## SYNTAX

```
Get-MgBetaServicePrincipalOwnerByRef -ServicePrincipalId <String> [-Filter <String>] [-Search <String>]
 [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>] [-ConsistencyLevel <String>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PageSize <Int32>] [-All]
 [-CountVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
Directory objects that are owners of this servicePrincipal.
The owners are a set of nonadmin users or servicePrincipals who are allowed to modify this object.
Supports $expand and $filter (/$count eq 0, /$count ne 0, /$count eq 1, /$count ne 1).

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Application.Read.All, Directory.ReadWrite.All, Directory.Read.All, Application.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Application.Read.All, Directory.ReadWrite.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All,  |

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

### -ConsistencyLevel
Indicates the requested consistency level.
Documentation URL: https://docs.microsoft.com/graph/aad-advanced-queries

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

### -ServicePrincipalId
The unique identifier of servicePrincipal

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
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

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/get-mgbetaserviceprincipalownerbyref](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/get-mgbetaserviceprincipalownerbyref)
























