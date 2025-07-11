---
external help file: Microsoft.Graph.Beta.Security-help.xml
Module Name: Microsoft.Graph.Beta.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecuritythreatintelligenceintelprofile
schema: 2.0.0
---

# New-MgBetaSecurityThreatIntelligenceIntelProfile

## SYNOPSIS
Create new navigation property to intelProfiles for security

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgSecurityThreatIntelligenceIntelProfile](/powershell/module/Microsoft.Graph.Security/New-MgSecurityThreatIntelligenceIntelProfile?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaSecurityThreatIntelligenceIntelProfile [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Aliases <String[]>]
 [-CountriesOrRegionsOfOrigin <IMicrosoftGraphSecurityIntelligenceProfileCountryOrRegionOfOrigin[]>]
 [-Description <IMicrosoftGraphSecurityFormattedContent>] [-FirstActiveDateTime <DateTime>] [-Id <String>]
 [-Indicators <IMicrosoftGraphSecurityIntelligenceProfileIndicator[]>] [-Kind <String>]
 [-Summary <IMicrosoftGraphSecurityFormattedContent>] [-Targets <String[]>] [-Title <String>]
 [-Tradecraft <IMicrosoftGraphSecurityFormattedContent>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaSecurityThreatIntelligenceIntelProfile -BodyParameter <IMicrosoftGraphSecurityIntelligenceProfile>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to intelProfiles for security

## EXAMPLES

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

### -Aliases
A list of commonly-known aliases for the threat intelligence included in the intelligenceProfile.

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

### -BodyParameter
intelligenceProfile
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityIntelligenceProfile
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

### -CountriesOrRegionsOfOrigin
The country/region of origin for the given actor or threat associated with this intelligenceProfile.
To construct, see NOTES section for COUNTRIESORREGIONSOFORIGIN properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityIntelligenceProfileCountryOrRegionOfOrigin[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
formattedContent
To construct, see NOTES section for DESCRIPTION properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityFormattedContent
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FirstActiveDateTime
The date and time when this intelligenceProfile was first active.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

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

### -Indicators
Includes an assemblage of high-fidelity network indicators of compromise.
To construct, see NOTES section for INDICATORS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityIntelligenceProfileIndicator[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Kind
intelligenceProfileKind

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

### -Summary
formattedContent
To construct, see NOTES section for SUMMARY properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityFormattedContent
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Targets
Known targets related to this intelligenceProfile.

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

### -Title
The title of this intelligenceProfile.

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

### -Tradecraft
formattedContent
To construct, see NOTES section for TRADECRAFT properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityFormattedContent
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSecurityIntelligenceProfile
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSecurityIntelligenceProfile
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphSecurityIntelligenceProfile>`: intelligenceProfile
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Aliases <String- `[]`>]`: A list of commonly-known aliases for the threat intelligence included in the intelligenceProfile.
  - `[CountriesOrRegionsOfOrigin <IMicrosoftGraphSecurityIntelligenceProfileCountryOrRegionOfOrigin- `[]`>]`: The country/region of origin for the given actor or threat associated with this intelligenceProfile.
    - `[Code <String>]`: A codified representation for this country/region of origin.
    - `[Label <String>]`: A display label for this ountry/region of origin.
  - `[Description <IMicrosoftGraphSecurityFormattedContent>]`: formattedContent
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Content <String>]`: The content of this formattedContent.
    - `[Format <String>]`: contentFormat
  - `[FirstActiveDateTime <DateTime?>]`: The date and time when this intelligenceProfile was first active. 
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[Indicators <IMicrosoftGraphSecurityIntelligenceProfileIndicator- `[]`>]`: Includes an assemblage of high-fidelity network indicators of compromise.
    - `[Artifact <IMicrosoftGraphSecurityArtifact>]`: artifact
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Source <String>]`: indicatorSource
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[FirstSeenDateTime <DateTime?>]`: Designate when an artifact was first used actively in an attack, when a particular sample was compiled, or if neither of those could be ascertained when the file was first seen in public repositories (for example, VirusTotal, ANY.RUN, Hybrid Analysis) or reported publicly.
    - `[LastSeenDateTime <DateTime?>]`: Designate when an artifact was most recently used actively in an attack, when a particular sample was compiled, or if neither of those could be ascertained when the file was first seen in public repositories (for example, VirusTotal, ANY.RUN, Hybrid Analysis) or reported publicly.
  - `[Kind <String>]`: intelligenceProfileKind
  - `[Summary <IMicrosoftGraphSecurityFormattedContent>]`: formattedContent
  - `[Targets <String- `[]`>]`: Known targets related to this intelligenceProfile.
  - `[Title <String>]`: The title of this intelligenceProfile.
  - `[Tradecraft <IMicrosoftGraphSecurityFormattedContent>]`: formattedContent

COUNTRIESORREGIONSOFORIGIN `<IMicrosoftGraphSecurityIntelligenceProfileCountryOrRegionOfOrigin- `[]`>`: The country/region of origin for the given actor or threat associated with this intelligenceProfile.
  - `[Code <String>]`: A codified representation for this country/region of origin.
  - `[Label <String>]`: A display label for this ountry/region of origin.

DESCRIPTION `<IMicrosoftGraphSecurityFormattedContent>`: formattedContent
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Content <String>]`: The content of this formattedContent.
  - `[Format <String>]`: contentFormat

INDICATORS `<IMicrosoftGraphSecurityIntelligenceProfileIndicator- `[]`>`: Includes an assemblage of high-fidelity network indicators of compromise.
  - `[Artifact <IMicrosoftGraphSecurityArtifact>]`: artifact
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Source <String>]`: indicatorSource
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[FirstSeenDateTime <DateTime?>]`: Designate when an artifact was first used actively in an attack, when a particular sample was compiled, or if neither of those could be ascertained when the file was first seen in public repositories (for example, VirusTotal, ANY.RUN, Hybrid Analysis) or reported publicly.
  - `[LastSeenDateTime <DateTime?>]`: Designate when an artifact was most recently used actively in an attack, when a particular sample was compiled, or if neither of those could be ascertained when the file was first seen in public repositories (for example, VirusTotal, ANY.RUN, Hybrid Analysis) or reported publicly.

SUMMARY `<IMicrosoftGraphSecurityFormattedContent>`: formattedContent
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Content <String>]`: The content of this formattedContent.
  - `[Format <String>]`: contentFormat

TRADECRAFT `<IMicrosoftGraphSecurityFormattedContent>`: formattedContent
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Content <String>]`: The content of this formattedContent.
  - `[Format <String>]`: contentFormat

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecuritythreatintelligenceintelprofile](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecuritythreatintelligenceintelprofile)
























