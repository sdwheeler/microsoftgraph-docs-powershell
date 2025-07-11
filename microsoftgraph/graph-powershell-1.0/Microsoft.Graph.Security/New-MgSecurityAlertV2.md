---
external help file: Microsoft.Graph.Security-help.xml
Module Name: Microsoft.Graph.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.security/new-mgsecurityalertv2
schema: 2.0.0
---

# New-MgSecurityAlertV2

## SYNOPSIS
Create new navigation property to alerts_v2 for security

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaSecurityAlertV2](/powershell/module/Microsoft.Graph.Beta.Security/New-MgBetaSecurityAlertV2?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgSecurityAlertV2 [-ResponseHeadersVariable <String>] [-ActorDisplayName <String>]
 [-AdditionalData <Hashtable>] [-AdditionalProperties <Hashtable>] [-AlertPolicyId <String>]
 [-AlertWebUrl <String>] [-AssignedTo <String>] [-Category <String>] [-Classification <String>]
 [-Comments <IMicrosoftGraphSecurityAlertComment[]>] [-CreatedDateTime <DateTime>] [-CustomDetails <Hashtable>]
 [-Description <String>] [-DetectionSource <String>] [-DetectorId <String>] [-Determination <String>]
 [-Evidence <IMicrosoftGraphSecurityAlertEvidence[]>] [-FirstActivityDateTime <DateTime>] [-Id <String>]
 [-IncidentId <String>] [-IncidentWebUrl <String>] [-LastActivityDateTime <DateTime>]
 [-LastUpdateDateTime <DateTime>] [-MitreTechniques <String[]>] [-ProductName <String>]
 [-ProviderAlertId <String>] [-RecommendedActions <String>] [-ResolvedDateTime <DateTime>]
 [-ServiceSource <String>] [-Severity <String>] [-Status <String>] [-SystemTags <String[]>]
 [-TenantId <String>] [-ThreatDisplayName <String>] [-ThreatFamilyName <String>] [-Title <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgSecurityAlertV2 -BodyParameter <IMicrosoftGraphSecurityAlert> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to alerts_v2 for security

## EXAMPLES

## PARAMETERS

### -ActorDisplayName
The adversary or activity group that is associated with this alert.

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

### -AdditionalData
dictionary

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

### -AlertPolicyId
The ID of the policy that generated the alert, and populated when there is a specific policy that generated the alert, whether configured by a customer or a built-in policy.

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

### -AlertWebUrl
URL for the Microsoft 365 Defender portal alert page.

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

### -AssignedTo
Owner of the alert, or null if no owner is assigned.

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
alert
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityAlert
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Category
The attack kill-chain category that the alert belongs to.
Aligned with the MITRE ATT&CK framework.

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

### -Classification
alertClassification

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

### -Comments
Array of comments created by the Security Operations (SecOps) team during the alert management process.
To construct, see NOTES section for COMMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityAlertComment[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
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

### -CreatedDateTime
Time when Microsoft 365 Defender created the alert.

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

### -CustomDetails
dictionary

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

### -Description
String value describing each alert.

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

### -DetectionSource
detectionSource

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

### -DetectorId
The ID of the detector that triggered the alert.

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

### -Determination
alertDetermination

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

### -Evidence
Collection of evidence related to the alert.
To construct, see NOTES section for EVIDENCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityAlertEvidence[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FirstActivityDateTime
The earliest activity associated with the alert.

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

### -IncidentId
Unique identifier to represent the incident this alert resource is associated with.

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

### -IncidentWebUrl
URL for the incident page in the Microsoft 365 Defender portal.

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

### -LastActivityDateTime
The oldest activity associated with the alert.

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

### -LastUpdateDateTime
Time when the alert was last updated at Microsoft 365 Defender.

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

### -MitreTechniques
The attack techniques, as aligned with the MITRE ATT&CK framework.

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

### -ProductName
The name of the product which published this alert.

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

### -ProviderAlertId
The ID of the alert as it appears in the security provider product that generated the alert.

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

### -RecommendedActions
Recommended response and remediation actions to take in the event this alert was generated.

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

### -ResolvedDateTime
Time when the alert was resolved.

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

### -ServiceSource
serviceSource

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

### -Severity
alertSeverity

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

### -Status
alertStatus

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

### -SystemTags
The system tags associated with the alert.

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

### -TenantId
The Microsoft Entra tenant the alert was created in.

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

### -ThreatDisplayName
The threat associated with this alert.

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

### -ThreatFamilyName
Threat family associated with this alert.

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

### -Title
Brief identifying string value describing the alert.

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphSecurityAlert
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphSecurityAlert
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphSecurityAlert>`: alert
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActorDisplayName <String>]`: The adversary or activity group that is associated with this alert.
  - `[AdditionalData <IMicrosoftGraphSecurityDictionary>]`: dictionary
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AlertPolicyId <String>]`: The ID of the policy that generated the alert, and populated when there is a specific policy that generated the alert, whether configured by a customer or a built-in policy.
  - `[AlertWebUrl <String>]`: URL for the Microsoft 365 Defender portal alert page.
  - `[AssignedTo <String>]`: Owner of the alert, or null if no owner is assigned.
  - `[Category <String>]`: The attack kill-chain category that the alert belongs to.
Aligned with the MITRE ATT&CK framework.
  - `[Classification <String>]`: alertClassification
  - `[Comments <IMicrosoftGraphSecurityAlertComment- `[]`>]`: Array of comments created by the Security Operations (SecOps) team during the alert management process.
    - `[Comment <String>]`: The comment text.
    - `[CreatedByDisplayName <String>]`: The person or app name that submitted the comment.
    - `[CreatedDateTime <DateTime?>]`: The time when the comment was submitted.
  - `[CreatedDateTime <DateTime?>]`: Time when Microsoft 365 Defender created the alert.
  - `[CustomDetails <IMicrosoftGraphSecurityDictionary>]`: dictionary
  - `[Description <String>]`: String value describing each alert.
  - `[DetectionSource <String>]`: detectionSource
  - `[DetectorId <String>]`: The ID of the detector that triggered the alert.
  - `[Determination <String>]`: alertDetermination
  - `[Evidence <IMicrosoftGraphSecurityAlertEvidence- `[]`>]`: Collection of evidence related to the alert.
    - `[CreatedDateTime <DateTime?>]`: The date and time when the evidence was created and added to the alert.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[DetailedRoles <String- `[]`>]`: Detailed description of the entity role/s in an alert.
Values are free-form.
    - `[RemediationStatus <String>]`: evidenceRemediationStatus
    - `[RemediationStatusDetails <String>]`: Details about the remediation status.
    - `[Roles <String- `[]`>]`: The role/s that an evidence entity represents in an alert, for example, an IP address that is associated with an attacker has the evidence role Attacker.
    - `[Tags <String- `[]`>]`: Array of custom tags associated with an evidence instance, for example, to denote a group of devices, high-value assets, etc.
    - `[Verdict <String>]`: evidenceVerdict
  - `[FirstActivityDateTime <DateTime?>]`: The earliest activity associated with the alert.
  - `[IncidentId <String>]`: Unique identifier to represent the incident this alert resource is associated with.
  - `[IncidentWebUrl <String>]`: URL for the incident page in the Microsoft 365 Defender portal.
  - `[LastActivityDateTime <DateTime?>]`: The oldest activity associated with the alert.
  - `[LastUpdateDateTime <DateTime?>]`: Time when the alert was last updated at Microsoft 365 Defender.
  - `[MitreTechniques <String- `[]`>]`: The attack techniques, as aligned with the MITRE ATT&CK framework.
  - `[ProductName <String>]`: The name of the product which published this alert.
  - `[ProviderAlertId <String>]`: The ID of the alert as it appears in the security provider product that generated the alert.
  - `[RecommendedActions <String>]`: Recommended response and remediation actions to take in the event this alert was generated.
  - `[ResolvedDateTime <DateTime?>]`: Time when the alert was resolved.
  - `[ServiceSource <String>]`: serviceSource
  - `[Severity <String>]`: alertSeverity
  - `[Status <String>]`: alertStatus
  - `[SystemTags <String- `[]`>]`: The system tags associated with the alert.
  - `[TenantId <String>]`: The Microsoft Entra tenant the alert was created in.
  - `[ThreatDisplayName <String>]`: The threat associated with this alert.
  - `[ThreatFamilyName <String>]`: Threat family associated with this alert.
  - `[Title <String>]`: Brief identifying string value describing the alert.

COMMENTS `<IMicrosoftGraphSecurityAlertComment- `[]`>`: Array of comments created by the Security Operations (SecOps) team during the alert management process.
  - `[Comment <String>]`: The comment text.
  - `[CreatedByDisplayName <String>]`: The person or app name that submitted the comment.
  - `[CreatedDateTime <DateTime?>]`: The time when the comment was submitted.

EVIDENCE `<IMicrosoftGraphSecurityAlertEvidence- `[]`>`: Collection of evidence related to the alert.
  - `[CreatedDateTime <DateTime?>]`: The date and time when the evidence was created and added to the alert.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[DetailedRoles <String- `[]`>]`: Detailed description of the entity role/s in an alert.
Values are free-form.
  - `[RemediationStatus <String>]`: evidenceRemediationStatus
  - `[RemediationStatusDetails <String>]`: Details about the remediation status.
  - `[Roles <String- `[]`>]`: The role/s that an evidence entity represents in an alert, for example, an IP address that is associated with an attacker has the evidence role Attacker.
  - `[Tags <String- `[]`>]`: Array of custom tags associated with an evidence instance, for example, to denote a group of devices, high-value assets, etc.
  - `[Verdict <String>]`: evidenceVerdict

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.security/new-mgsecurityalertv2](https://learn.microsoft.com/powershell/module/microsoft.graph.security/new-mgsecurityalertv2)
























