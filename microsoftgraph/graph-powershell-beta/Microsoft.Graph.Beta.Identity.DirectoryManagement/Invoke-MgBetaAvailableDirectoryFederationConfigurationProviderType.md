---
external help file: Microsoft.Graph.Beta.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Beta.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/invoke-mgbetaavailabledirectoryfederationconfigurationprovidertype
schema: 2.0.0
ms.subservice: entra-sign-in
---

# Invoke-MgBetaAvailableDirectoryFederationConfigurationProviderType

## SYNOPSIS
Get all identity providers supported in a directory.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Invoke-MgAvailableDirectoryFederationConfigurationProviderType](/powershell/module/Microsoft.Graph.Identity.DirectoryManagement/Invoke-MgAvailableDirectoryFederationConfigurationProviderType?view=graph-powershell-1.0)

## SYNTAX

```
Invoke-MgBetaAvailableDirectoryFederationConfigurationProviderType [-Count] [-Filter <String>]
 [-Search <String>] [-Skip <Int32>] [-Top <Int32>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Get all identity providers supported in a directory.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | IdentityProvider.Read.All, IdentityProvider.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | IdentityProvider.Read.All, IdentityProvider.ReadWrite.All,  |

## EXAMPLES

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

### System.String
## NOTES

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/invoke-mgbetaavailabledirectoryfederationconfigurationprovidertype](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/invoke-mgbetaavailabledirectoryfederationconfigurationprovidertype)

[https://learn.microsoft.com/graph/api/identityproviderbase-availableprovidertypes?view=graph-rest-beta](https://learn.microsoft.com/graph/api/identityproviderbase-availableprovidertypes?view=graph-rest-beta)
























