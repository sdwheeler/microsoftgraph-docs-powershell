---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgserviceprincipalriskdetection
schema: 2.0.0
---

# New-MgServicePrincipalRiskDetection

## SYNOPSIS
Create new navigation property to servicePrincipalRiskDetections for identityProtection

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaServicePrincipalRiskDetection](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/New-MgBetaServicePrincipalRiskDetection?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgServicePrincipalRiskDetection [-ResponseHeadersVariable <String>] [-Activity <String>]
 [-ActivityDateTime <DateTime>] [-AdditionalInfo <String>] [-AdditionalProperties <Hashtable>]
 [-AppId <String>] [-CorrelationId <String>] [-DetectedDateTime <DateTime>] [-DetectionTimingType <String>]
 [-IPAddress <String>] [-Id <String>] [-KeyIds <String[]>] [-LastUpdatedDateTime <DateTime>]
 [-Location <IMicrosoftGraphSignInLocation>] [-RequestId <String>] [-RiskDetail <String>]
 [-RiskEventType <String>] [-RiskLevel <String>] [-RiskState <String>] [-ServicePrincipalDisplayName <String>]
 [-ServicePrincipalId <String>] [-Source <String>] [-TokenIssuerType <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgServicePrincipalRiskDetection -BodyParameter <IMicrosoftGraphServicePrincipalRiskDetection>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to servicePrincipalRiskDetections for identityProtection

## EXAMPLES

## PARAMETERS

### -Activity
activityType

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

### -ActivityDateTime
Date and time when the risky activity occurred.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z

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

### -AdditionalInfo
Additional information associated with the risk detection.
This string value is represented as a JSON object with the quotations escaped.

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

### -AppId
The unique identifier for the associated application.

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
servicePrincipalRiskDetection
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphServicePrincipalRiskDetection
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

### -CorrelationId
Correlation ID of the sign-in activity associated with the risk detection.
This property is null if the risk detection is not associated with a sign-in activity.

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

### -DetectedDateTime
Date and time when the risk was detected.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
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

### -DetectionTimingType
riskDetectionTimingType

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

### -IPAddress
Provides the IP address of the client from where the risk occurred.

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

### -KeyIds
The unique identifier for the key credential associated with the risk detection.

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

### -LastUpdatedDateTime
Date and time when the risk detection was last updated.

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

### -Location
signInLocation
To construct, see NOTES section for LOCATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphSignInLocation
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RequestId
Request identifier of the sign-in activity associated with the risk detection.
This property is null if the risk detection is not associated with a sign-in activity.
Supports $filter (eq).

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

### -RiskDetail
riskDetail

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

### -RiskEventType
The type of risk event detected.
The possible values are: investigationsThreatIntelligence, generic, adminConfirmedServicePrincipalCompromised, suspiciousSignins, leakedCredentials, anomalousServicePrincipalActivity, maliciousApplication, suspiciousApplication.

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

### -RiskLevel
riskLevel

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

### -RiskState
riskState

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

### -ServicePrincipalDisplayName
The display name for the service principal.

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

### -ServicePrincipalId
The unique identifier for the service principal.
Supports $filter (eq).

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

### -Source
Source of the risk detection.
For example, identityProtection.

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

### -TokenIssuerType
tokenIssuerType

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphServicePrincipalRiskDetection
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphServicePrincipalRiskDetection
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphServicePrincipalRiskDetection>`: servicePrincipalRiskDetection
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Activity <String>]`: activityType
  - `[ActivityDateTime <DateTime?>]`: Date and time when the risky activity occurred.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[AdditionalInfo <String>]`: Additional information associated with the risk detection.
This string value is represented as a JSON object with the quotations escaped.
  - `[AppId <String>]`: The unique identifier for the associated application.
  - `[CorrelationId <String>]`: Correlation ID of the sign-in activity associated with the risk detection.
This property is null if the risk detection is not associated with a sign-in activity.
  - `[DetectedDateTime <DateTime?>]`: Date and time when the risk was detected.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[DetectionTimingType <String>]`: riskDetectionTimingType
  - `[IPAddress <String>]`: Provides the IP address of the client from where the risk occurred.
  - `[KeyIds <String- `[]`>]`: The unique identifier for the key credential associated with the risk detection.
  - `[LastUpdatedDateTime <DateTime?>]`: Date and time when the risk detection was last updated.
  - `[Location <IMicrosoftGraphSignInLocation>]`: signInLocation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[City <String>]`: Provides the city where the sign-in originated and is determined using latitude/longitude information from the sign-in activity.
    - `[CountryOrRegion <String>]`: Provides the country code info (two letter code) where the sign-in originated.
This is calculated using latitude/longitude information from the sign-in activity.
    - `[GeoCoordinates <IMicrosoftGraphGeoCoordinates>]`: geoCoordinates
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Altitude <Double?>]`: Optional.
The altitude (height), in feet,  above sea level for the item.
Read-only.
      - `[Latitude <Double?>]`: Optional.
The latitude, in decimal, for the item.
Read-only.
      - `[Longitude <Double?>]`: Optional.
The longitude, in decimal, for the item.
Read-only.
    - `[State <String>]`: Provides the State where the sign-in originated.
This is calculated using latitude/longitude information from the sign-in activity.
  - `[RequestId <String>]`: Request identifier of the sign-in activity associated with the risk detection.
This property is null if the risk detection is not associated with a sign-in activity.
Supports $filter (eq).
  - `[RiskDetail <String>]`: riskDetail
  - `[RiskEventType <String>]`: The type of risk event detected.
The possible values are: investigationsThreatIntelligence, generic, adminConfirmedServicePrincipalCompromised, suspiciousSignins, leakedCredentials, anomalousServicePrincipalActivity, maliciousApplication, suspiciousApplication.
  - `[RiskLevel <String>]`: riskLevel
  - `[RiskState <String>]`: riskState
  - `[ServicePrincipalDisplayName <String>]`: The display name for the service principal.
  - `[ServicePrincipalId <String>]`: The unique identifier for the service principal.
Supports $filter (eq).
  - `[Source <String>]`: Source of the risk detection.
For example, identityProtection.
  - `[TokenIssuerType <String>]`: tokenIssuerType

LOCATION `<IMicrosoftGraphSignInLocation>`: signInLocation
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[City <String>]`: Provides the city where the sign-in originated and is determined using latitude/longitude information from the sign-in activity.
  - `[CountryOrRegion <String>]`: Provides the country code info (two letter code) where the sign-in originated.
This is calculated using latitude/longitude information from the sign-in activity.
  - `[GeoCoordinates <IMicrosoftGraphGeoCoordinates>]`: geoCoordinates
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Altitude <Double?>]`: Optional.
The altitude (height), in feet,  above sea level for the item.
Read-only.
    - `[Latitude <Double?>]`: Optional.
The latitude, in decimal, for the item.
Read-only.
    - `[Longitude <Double?>]`: Optional.
The longitude, in decimal, for the item.
Read-only.
  - `[State <String>]`: Provides the State where the sign-in originated.
This is calculated using latitude/longitude information from the sign-in activity.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgserviceprincipalriskdetection](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgserviceprincipalriskdetection)
























