---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgidentityconditionalaccessnamedlocation
schema: 2.0.0
ms.subservice: entra-sign-in
---

# New-MgIdentityConditionalAccessNamedLocation

## SYNOPSIS
Create a new namedLocation object.
Named locations can be either ipNamedLocation or countryNamedLocation objects.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaIdentityConditionalAccessNamedLocation](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/New-MgBetaIdentityConditionalAccessNamedLocation?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgIdentityConditionalAccessNamedLocation [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>] [-DisplayName <String>] [-Id <String>]
 [-ModifiedDateTime <DateTime>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgIdentityConditionalAccessNamedLocation -BodyParameter <IMicrosoftGraphNamedLocation>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new namedLocation object.
Named locations can be either ipNamedLocation or countryNamedLocation objects.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Policy.Read.All, Policy.ReadWrite.ConditionalAccess,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Policy.Read.All, Policy.ReadWrite.ConditionalAccess,  |

## EXAMPLES
### Example 1: Create a country named location

```powershell
Connect-MgGraph -Scopes 'Policy.ReadWrite.ConditionalAccess'

$params = @{
"@odata.type" = "#microsoft.graph.countryNamedLocation"
DisplayName = "Named location with unknown countries and regions"
CountriesAndRegions = @(
    "US"
    "XK"
)
IncludeUnknownCountriesAndRegions = $true
}

New-MgIdentityConditionalAccessNamedLocation -BodyParameter $params

Id                                   CreatedDateTime      DisplayName                                       ModifiedDateTime
--                                   ---------------      -----------                                       ----------------
1f0fd623-bf8f-4003-9627-32a68c3cdcc1 6/13/2022 8:27:35 AM Named location with unknown countries and regions 6/13/2022 8:27:35 AM
```

This example creates a country named location.

### Example 2: Create an ip named location

```powershell
Connect-MgGraph -Scopes 'Policy.ReadWrite.ConditionalAccess'

$params = @{
"@odata.type" = "#microsoft.graph.ipNamedLocation"
DisplayName = "Untrusted IP named location"
IsTrusted = $false
IpRanges = @(
    @{
        "@odata.type" = "#microsoft.graph.iPv4CidrRange"
        CidrAddress = "12.34.221.11/22"
    }
    @{
        "@odata.type" = "#microsoft.graph.iPv6CidrRange"
        CidrAddress = "2001:0:9d38:90d6:0:0:0:0/63"
    }
)
}

New-MgIdentityConditionalAccessNamedLocation -BodyParameter $params

Id                                   CreatedDateTime      DisplayName                 ModifiedDateTime
--                                   ---------------      -----------                 ----------------
0824dbaf-6277-4db0-8112-b29fd356f2c4 6/13/2022 8:41:38 AM Untrusted IP named location 6/13/2022 8:41:38 AM
```

This example creates an Ip named location.

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
namedLocation
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphNamedLocation
Parameter Sets: Create
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

### -CreatedDateTime
The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Human-readable name of the location.

```yaml
Type: String
Parameter Sets: CreateExpanded
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
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ModifiedDateTime
The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphNamedLocation
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphNamedLocation
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphNamedLocation>`: namedLocation
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
  - `[DisplayName <String>]`: Human-readable name of the location.
  - `[ModifiedDateTime <DateTime?>]`: The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgidentityconditionalaccessnamedlocation](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgidentityconditionalaccessnamedlocation)

[https://learn.microsoft.com/graph/api/conditionalaccessroot-post-namedlocations?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/conditionalaccessroot-post-namedlocations?view=graph-rest-1.0)























