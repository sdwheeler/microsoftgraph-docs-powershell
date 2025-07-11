---
external help file: Microsoft.Graph.Beta.Security-help.xml
Module Name: Microsoft.Graph.Beta.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecurityipsecurityprofile
schema: 2.0.0
---

# New-MgBetaSecurityIPSecurityProfile

## SYNOPSIS
Create new navigation property to ipSecurityProfiles for security

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaSecurityIPSecurityProfile [-ResponseHeadersVariable <String>] [-ActivityGroupNames <String[]>]
 [-AdditionalProperties <Hashtable>] [-Address <String>] [-AzureSubscriptionId <String>]
 [-AzureTenantId <String>] [-CountHits <Int32>] [-CountHosts <Int32>] [-FirstSeenDateTime <DateTime>]
 [-IPCategories <IMicrosoftGraphIPCategory[]>] [-IPReferenceData <IMicrosoftGraphIPReferenceData[]>]
 [-Id <String>] [-LastSeenDateTime <DateTime>] [-RiskScore <String>] [-Tags <String[]>]
 [-VendorInformation <IMicrosoftGraphSecurityVendorInformation>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaSecurityIPSecurityProfile -BodyParameter <IMicrosoftGraphIPSecurityProfile>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to ipSecurityProfiles for security

## EXAMPLES

## PARAMETERS

### -ActivityGroupNames


```yaml
Type: String[]
Parameter Sets: CreateExpanded
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
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Address


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

### -AzureSubscriptionId


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

### -AzureTenantId


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

### -BodyParameter
ipSecurityProfile
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphIPSecurityProfile
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

### -CountHits


```yaml
Type: Int32
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -CountHosts


```yaml
Type: Int32
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -FirstSeenDateTime


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

### -IPCategories

To construct, see NOTES section for IPCATEGORIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphIPCategory[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IPReferenceData

To construct, see NOTES section for IPREFERENCEDATA properties and create a hash table.

```yaml
Type: IMicrosoftGraphIPReferenceData[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastSeenDateTime


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

### -RiskScore


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

### -Tags


```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VendorInformation
securityVendorInformation
To construct, see NOTES section for VENDORINFORMATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityVendorInformation
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphIPSecurityProfile
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphIPSecurityProfile
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphIPSecurityProfile>`: ipSecurityProfile
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActivityGroupNames <String- `[]`>]`: 
  - `[Address <String>]`: 
  - `[AzureSubscriptionId <String>]`: 
  - `[AzureTenantId <String>]`: 
  - `[CountHits <Int32?>]`: 
  - `[CountHosts <Int32?>]`: 
  - `[FirstSeenDateTime <DateTime?>]`: 
  - `[IPCategories <IMicrosoftGraphIPCategory- `[]`>]`: 
    - `[Description <String>]`: 
    - `[Name <String>]`: 
    - `[Vendor <String>]`: 
  - `[IPReferenceData <IMicrosoftGraphIPReferenceData- `[]`>]`: 
    - `[Asn <Int64?>]`: 
    - `[City <String>]`: 
    - `[CountryOrRegionCode <String>]`: 
    - `[Organization <String>]`: 
    - `[State <String>]`: 
    - `[Vendor <String>]`: 
  - `[LastSeenDateTime <DateTime?>]`: 
  - `[RiskScore <String>]`: 
  - `[Tags <String- `[]`>]`: 
  - `[VendorInformation <IMicrosoftGraphSecurityVendorInformation>]`: securityVendorInformation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Provider <String>]`: Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.
    - `[ProviderVersion <String>]`: Version of the provider or subprovider, if it exists, that generated the alert.
Required
    - `[SubProvider <String>]`: Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.
    - `[Vendor <String>]`: Name of the alert vendor (for example, Microsoft, Dell, FireEye).
Required

IPCATEGORIES `<IMicrosoftGraphIPCategory- `[]`>`: .
  - `[Description <String>]`: 
  - `[Name <String>]`: 
  - `[Vendor <String>]`: 

IPREFERENCEDATA `<IMicrosoftGraphIPReferenceData- `[]`>`: .
  - `[Asn <Int64?>]`: 
  - `[City <String>]`: 
  - `[CountryOrRegionCode <String>]`: 
  - `[Organization <String>]`: 
  - `[State <String>]`: 
  - `[Vendor <String>]`: 

VENDORINFORMATION `<IMicrosoftGraphSecurityVendorInformation>`: securityVendorInformation
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Provider <String>]`: Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.
  - `[ProviderVersion <String>]`: Version of the provider or subprovider, if it exists, that generated the alert.
Required
  - `[SubProvider <String>]`: Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.
  - `[Vendor <String>]`: Name of the alert vendor (for example, Microsoft, Dell, FireEye).
Required

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecurityipsecurityprofile](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecurityipsecurityprofile)
























