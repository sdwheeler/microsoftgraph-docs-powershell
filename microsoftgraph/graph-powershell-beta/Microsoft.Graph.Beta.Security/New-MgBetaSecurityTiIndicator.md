---
external help file: Microsoft.Graph.Beta.Security-help.xml
Module Name: Microsoft.Graph.Beta.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecuritytiindicator
schema: 2.0.0
ms.subservice: security
---

# New-MgBetaSecurityTiIndicator

## SYNOPSIS
Create a new tiIndicator object.

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaSecurityTiIndicator [-ResponseHeadersVariable <String>] [-Action <String>]
 [-ActivityGroupNames <String[]>] [-AdditionalInformation <String>] [-AdditionalProperties <Hashtable>]
 [-AzureTenantId <String>] [-Confidence <Int32>] [-Description <String>] [-DiamondModel <String>]
 [-DomainName <String>] [-EmailEncoding <String>] [-EmailLanguage <String>] [-EmailRecipient <String>]
 [-EmailSenderAddress <String>] [-EmailSenderName <String>] [-EmailSourceDomain <String>]
 [-EmailSourceIPAddress <String>] [-EmailSubject <String>] [-EmailXMailer <String>]
 [-ExpirationDateTime <DateTime>] [-ExternalId <String>] [-FileCompileDateTime <DateTime>]
 [-FileCreatedDateTime <DateTime>] [-FileHashType <String>] [-FileHashValue <String>] [-FileMutexName <String>]
 [-FileName <String>] [-FilePacker <String>] [-FilePath <String>] [-FileSize <Int64>] [-FileType <String>]
 [-Id <String>] [-IngestedDateTime <DateTime>] [-IsActive] [-KillChain <String[]>]
 [-KnownFalsePositives <String>] [-LastReportedDateTime <DateTime>] [-MalwareFamilyNames <String[]>]
 [-NetworkCidrBlock <String>] [-NetworkDestinationAsn <Int64>] [-NetworkDestinationCidrBlock <String>]
 [-NetworkDestinationIPv4 <String>] [-NetworkDestinationIPv6 <String>] [-NetworkDestinationPort <Int32>]
 [-NetworkIPv4 <String>] [-NetworkIPv6 <String>] [-NetworkPort <Int32>] [-NetworkProtocol <Int32>]
 [-NetworkSourceAsn <Int64>] [-NetworkSourceCidrBlock <String>] [-NetworkSourceIPv4 <String>]
 [-NetworkSourceIPv6 <String>] [-NetworkSourcePort <Int32>] [-PassiveOnly] [-Severity <Int32>]
 [-Tags <String[]>] [-TargetProduct <String>] [-ThreatType <String>] [-TlpLevel <String>] [-Url <String>]
 [-UserAgent <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgBetaSecurityTiIndicator -BodyParameter <IMicrosoftGraphTiIndicator> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new tiIndicator object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | ThreatIndicators.ReadWrite.OwnedBy,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | ThreatIndicators.ReadWrite.OwnedBy,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	action = "alert"
	activityGroupNames = @(
	)
	confidence = 0
	description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator."
	expirationDateTime = [System.DateTime]::Parse("2019-03-01T21:43:37.5031462+00:00")
	externalId = "Test--8586509942679764298MS501"
	fileHashType = "sha256"
	fileHashValue = "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313"
	killChain = @(
	)
	malwareFamilyNames = @(
	)
	severity = 0
	tags = @(
	)
	targetProduct = "Azure Sentinel"
	threatType = "WatchList"
	tlpLevel = "green"
}

New-MgBetaSecurityTiIndicator -BodyParameter $params

```
This example shows how to use the New-MgBetaSecurityTiIndicator Cmdlet.


## PARAMETERS

### -Action
tiAction

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

### -ActivityGroupNames
The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.

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

### -AdditionalInformation
A catchall area for extra data from the indicator that is not specifically covered by other tiIndicator properties.
The security tool specified by targetProduct typically does not utilize this data.

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

### -AzureTenantId
Stamped by the system when the indicator is ingested.
The Microsoft Entra tenant id of submitting client.
Required.

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
tiIndicator
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTiIndicator
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confidence
An integer representing the confidence the data within the indicator accurately identifies malicious behavior.
Acceptable values are 0 - 100 with 100 being the highest.

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

### -Description
Brief description (100 characters or less) of the threat represented by the indicator.
Required.

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

### -DiamondModel
diamondModel

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

### -DomainName


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

### -EmailEncoding


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

### -EmailLanguage


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

### -EmailRecipient


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

### -EmailSenderAddress


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

### -EmailSenderName


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

### -EmailSourceDomain


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

### -EmailSourceIPAddress


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

### -EmailSubject


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

### -EmailXMailer


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

### -ExpirationDateTime
DateTime string indicating when the Indicator expires.
All indicators must have an expiration date to avoid stale indicators persisting in the system.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Required.

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

### -ExternalId
An identification number that ties the indicator back to the indicator provider's system (for example, a foreign key).

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

### -FileCompileDateTime


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

### -FileCreatedDateTime


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

### -FileHashType
fileHashType

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

### -FileHashValue


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

### -FileMutexName


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

### -FileName


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

### -FilePacker


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

### -FilePath


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

### -FileSize


```yaml
Type: Int64
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -FileType


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

### -IngestedDateTime
Stamped by the system when the indicator is ingested.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
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

### -IsActive
Used to deactivate indicators within system.
By default, any indicator submitted is set as active.
However, providers may submit existing indicators with this set to 'False' to deactivate indicators in the system.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -KillChain
A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.
See 'killChain values' below for exact values.

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

### -KnownFalsePositives
Scenarios in which the indicator may cause false positives.
This should be human-readable text.

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

### -LastReportedDateTime
The last time the indicator was seen.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
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

### -MalwareFamilyNames
The malware family name associated with an indicator if it exists.
Microsoft prefers the Microsoft malware family name if at all possible that can be found via the Windows Defender Security Intelligence threat encyclopedia.

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

### -NetworkCidrBlock


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

### -NetworkDestinationAsn


```yaml
Type: Int64
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkDestinationCidrBlock


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

### -NetworkDestinationIPv4


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

### -NetworkDestinationIPv6


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

### -NetworkDestinationPort


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

### -NetworkIPv4


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

### -NetworkIPv6


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

### -NetworkPort


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

### -NetworkProtocol


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

### -NetworkSourceAsn


```yaml
Type: Int64
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkSourceCidrBlock


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

### -NetworkSourceIPv4


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

### -NetworkSourceIPv6


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

### -NetworkSourcePort


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

### -PassiveOnly
Determines if the indicator should trigger an event that is visible to an end-user.
When set to 'true,' security tools won't notify the end user that a 'hit' has occurred.
This is most often treated as audit or silent mode by security products where they'll simply log that a match occurred but won't perform the action.
Default value is false.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
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

### -Severity
An integer representing the severity of the malicious behavior identified by the data within the indicator.
Acceptable values are 0 - 5 where 5 is the most severe and zero isn't severe at all.
Default value is 3.

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

### -Tags
A JSON array of strings that stores arbitrary tags/keywords.

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

### -TargetProduct
A string value representing a single security product to which the indicator should be applied.
Acceptable values are: Azure Sentinel, Microsoft Defender ATP.
Required

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

### -ThreatType
Each indicator must have a valid Indicator Threat Type.
Possible values are: Botnet, C2, CryptoMining, Darknet, DDoS, MaliciousUrl, Malware, Phishing, Proxy, PUA, WatchList.
Required.

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

### -TlpLevel
tlpLevel

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

### -Url


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

### -UserAgent


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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphTiIndicator
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphTiIndicator
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphTiIndicator>`: tiIndicator
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Action <String>]`: tiAction
  - `[ActivityGroupNames <String- `[]`>]`: The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.
  - `[AdditionalInformation <String>]`: A catchall area for extra data from the indicator that is not specifically covered by other tiIndicator properties.
The security tool specified by targetProduct typically does not utilize this data.
  - `[AzureTenantId <String>]`: Stamped by the system when the indicator is ingested.
The Microsoft Entra tenant id of submitting client.
Required.
  - `[Confidence <Int32?>]`: An integer representing the confidence the data within the indicator accurately identifies malicious behavior.
Acceptable values are 0 - 100 with 100 being the highest.
  - `[Description <String>]`: Brief description (100 characters or less) of the threat represented by the indicator.
Required.
  - `[DiamondModel <String>]`: diamondModel
  - `[DomainName <String>]`: 
  - `[EmailEncoding <String>]`: 
  - `[EmailLanguage <String>]`: 
  - `[EmailRecipient <String>]`: 
  - `[EmailSenderAddress <String>]`: 
  - `[EmailSenderName <String>]`: 
  - `[EmailSourceDomain <String>]`: 
  - `[EmailSourceIPAddress <String>]`: 
  - `[EmailSubject <String>]`: 
  - `[EmailXMailer <String>]`: 
  - `[ExpirationDateTime <DateTime?>]`: DateTime string indicating when the Indicator expires.
All indicators must have an expiration date to avoid stale indicators persisting in the system.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Required.
  - `[ExternalId <String>]`: An identification number that ties the indicator back to the indicator provider's system (for example, a foreign key).
  - `[FileCompileDateTime <DateTime?>]`: 
  - `[FileCreatedDateTime <DateTime?>]`: 
  - `[FileHashType <String>]`: fileHashType
  - `[FileHashValue <String>]`: 
  - `[FileMutexName <String>]`: 
  - `[FileName <String>]`: 
  - `[FilePacker <String>]`: 
  - `[FilePath <String>]`: 
  - `[FileSize <Int64?>]`: 
  - `[FileType <String>]`: 
  - `[IngestedDateTime <DateTime?>]`: Stamped by the system when the indicator is ingested.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[IsActive <Boolean?>]`: Used to deactivate indicators within system.
By default, any indicator submitted is set as active.
However, providers may submit existing indicators with this set to 'False' to deactivate indicators in the system.
  - `[KillChain <String- `[]`>]`: A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.
See 'killChain values' below for exact values.
  - `[KnownFalsePositives <String>]`: Scenarios in which the indicator may cause false positives.
This should be human-readable text.
  - `[LastReportedDateTime <DateTime?>]`: The last time the indicator was seen.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[MalwareFamilyNames <String- `[]`>]`: The malware family name associated with an indicator if it exists.
Microsoft prefers the Microsoft malware family name if at all possible that can be found via the Windows Defender Security Intelligence threat encyclopedia.
  - `[NetworkCidrBlock <String>]`: 
  - `[NetworkDestinationAsn <Int64?>]`: 
  - `[NetworkDestinationCidrBlock <String>]`: 
  - `[NetworkDestinationIPv4 <String>]`: 
  - `[NetworkDestinationIPv6 <String>]`: 
  - `[NetworkDestinationPort <Int32?>]`: 
  - `[NetworkIPv4 <String>]`: 
  - `[NetworkIPv6 <String>]`: 
  - `[NetworkPort <Int32?>]`: 
  - `[NetworkProtocol <Int32?>]`: 
  - `[NetworkSourceAsn <Int64?>]`: 
  - `[NetworkSourceCidrBlock <String>]`: 
  - `[NetworkSourceIPv4 <String>]`: 
  - `[NetworkSourceIPv6 <String>]`: 
  - `[NetworkSourcePort <Int32?>]`: 
  - `[PassiveOnly <Boolean?>]`: Determines if the indicator should trigger an event that is visible to an end-user.
When set to 'true,' security tools won't notify the end user that a 'hit' has occurred.
This is most often treated as audit or silent mode by security products where they'll simply log that a match occurred but won't perform the action.
Default value is false.
  - `[Severity <Int32?>]`: An integer representing the severity of the malicious behavior identified by the data within the indicator.
Acceptable values are 0 - 5 where 5 is the most severe and zero isn't severe at all.
Default value is 3.
  - `[Tags <String- `[]`>]`: A JSON array of strings that stores arbitrary tags/keywords.
  - `[TargetProduct <String>]`: A string value representing a single security product to which the indicator should be applied.
Acceptable values are: Azure Sentinel, Microsoft Defender ATP.
Required
  - `[ThreatType <String>]`: Each indicator must have a valid Indicator Threat Type.
Possible values are: Botnet, C2, CryptoMining, Darknet, DDoS, MaliciousUrl, Malware, Phishing, Proxy, PUA, WatchList.
Required.
  - `[TlpLevel <String>]`: tlpLevel
  - `[Url <String>]`: 
  - `[UserAgent <String>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecuritytiindicator](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecuritytiindicator)

[https://learn.microsoft.com/graph/api/tiindicators-post?view=graph-rest-beta](https://learn.microsoft.com/graph/api/tiindicators-post?view=graph-rest-beta)























