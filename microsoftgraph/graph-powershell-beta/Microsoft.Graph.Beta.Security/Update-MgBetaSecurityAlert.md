---
external help file: Microsoft.Graph.Beta.Security-help.xml
Module Name: Microsoft.Graph.Beta.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/update-mgbetasecurityalert
schema: 2.0.0
ms.subservice: security
---

# Update-MgBetaSecurityAlert

## SYNOPSIS
Update an editable alert property within any integrated solution to keep alert status and assignments in sync across solutions.
This method updates any solution that has a record of the referenced alert ID.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgSecurityAlert](/powershell/module/Microsoft.Graph.Security/Update-MgSecurityAlert?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaSecurityAlert -AlertId <String> [-ResponseHeadersVariable <String>] [-ActivityGroupName <String>]
 [-AdditionalProperties <Hashtable>] [-AlertDetections <IMicrosoftGraphAlertDetection[]>]
 [-AssignedTo <String>] [-AzureSubscriptionId <String>] [-AzureTenantId <String>] [-Category <String>]
 [-ClosedDateTime <DateTime>] [-CloudAppStates <IMicrosoftGraphCloudAppSecurityState[]>] [-Comments <String[]>]
 [-Confidence <Int32>] [-CreatedDateTime <DateTime>] [-Description <String>] [-DetectionIds <String[]>]
 [-EventDateTime <DateTime>] [-Feedback <String>] [-FileStates <IMicrosoftGraphFileSecurityState[]>]
 [-HistoryStates <IMicrosoftGraphAlertHistoryState[]>] [-HostStates <IMicrosoftGraphHostSecurityState[]>]
 [-Id <String>] [-IncidentIds <String[]>]
 [-InvestigationSecurityStates <IMicrosoftGraphInvestigationSecurityState[]>] [-LastEventDateTime <DateTime>]
 [-LastModifiedDateTime <DateTime>] [-MalwareStates <IMicrosoftGraphMalwareState[]>]
 [-MessageSecurityStates <IMicrosoftGraphMessageSecurityState[]>]
 [-NetworkConnections <IMicrosoftGraphNetworkConnection[]>] [-Processes <IMicrosoftGraphProcess[]>]
 [-RecommendedActions <String[]>] [-RegistryKeyStates <IMicrosoftGraphRegistryKeyState[]>]
 [-SecurityResources <IMicrosoftGraphSecurityResource[]>] [-Severity <String>] [-SourceMaterials <String[]>]
 [-Status <String>] [-Tags <String[]>] [-Title <String>] [-Triggers <IMicrosoftGraphAlertTrigger[]>]
 [-UriClickSecurityStates <IMicrosoftGraphUriClickSecurityState[]>]
 [-UserStates <IMicrosoftGraphUserSecurityState[]>]
 [-VendorInformation <IMicrosoftGraphSecurityVendorInformation>]
 [-VulnerabilityStates <IMicrosoftGraphVulnerabilityState[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaSecurityAlert -AlertId <String> -BodyParameter <IMicrosoftGraphAlert>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaSecurityAlert -InputObject <ISecurityIdentity> [-ResponseHeadersVariable <String>]
 [-ActivityGroupName <String>] [-AdditionalProperties <Hashtable>]
 [-AlertDetections <IMicrosoftGraphAlertDetection[]>] [-AssignedTo <String>] [-AzureSubscriptionId <String>]
 [-AzureTenantId <String>] [-Category <String>] [-ClosedDateTime <DateTime>]
 [-CloudAppStates <IMicrosoftGraphCloudAppSecurityState[]>] [-Comments <String[]>] [-Confidence <Int32>]
 [-CreatedDateTime <DateTime>] [-Description <String>] [-DetectionIds <String[]>] [-EventDateTime <DateTime>]
 [-Feedback <String>] [-FileStates <IMicrosoftGraphFileSecurityState[]>]
 [-HistoryStates <IMicrosoftGraphAlertHistoryState[]>] [-HostStates <IMicrosoftGraphHostSecurityState[]>]
 [-Id <String>] [-IncidentIds <String[]>]
 [-InvestigationSecurityStates <IMicrosoftGraphInvestigationSecurityState[]>] [-LastEventDateTime <DateTime>]
 [-LastModifiedDateTime <DateTime>] [-MalwareStates <IMicrosoftGraphMalwareState[]>]
 [-MessageSecurityStates <IMicrosoftGraphMessageSecurityState[]>]
 [-NetworkConnections <IMicrosoftGraphNetworkConnection[]>] [-Processes <IMicrosoftGraphProcess[]>]
 [-RecommendedActions <String[]>] [-RegistryKeyStates <IMicrosoftGraphRegistryKeyState[]>]
 [-SecurityResources <IMicrosoftGraphSecurityResource[]>] [-Severity <String>] [-SourceMaterials <String[]>]
 [-Status <String>] [-Tags <String[]>] [-Title <String>] [-Triggers <IMicrosoftGraphAlertTrigger[]>]
 [-UriClickSecurityStates <IMicrosoftGraphUriClickSecurityState[]>]
 [-UserStates <IMicrosoftGraphUserSecurityState[]>]
 [-VendorInformation <IMicrosoftGraphSecurityVendorInformation>]
 [-VulnerabilityStates <IMicrosoftGraphVulnerabilityState[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaSecurityAlert -InputObject <ISecurityIdentity> -BodyParameter <IMicrosoftGraphAlert>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update an editable alert property within any integrated solution to keep alert status and assignments in sync across solutions.
This method updates any solution that has a record of the referenced alert ID.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | SecurityEvents.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | SecurityEvents.ReadWrite.All,  |

## EXAMPLES
### Example 1: Request without Prefer header

```powershell

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	assignedTo = "String"
	closedDateTime = [System.DateTime]::Parse("String (timestamp)")
	comments = @(
		"String"
	)
	feedback = "@odata.type: microsoft.graph.alertFeedback"
	status = "@odata.type: microsoft.graph.alertStatus"
	tags = @(
		"String"
	)
	vendorInformation = @{
		provider = "String"
		vendor = "String"
	}
}

Update-MgBetaSecurityAlert -AlertId $alertId -BodyParameter $params

```
This example will request without prefer header

### Example 2: Request with Prefer header

```powershell

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	assignedTo = "String"
	closedDateTime = [System.DateTime]::Parse("String (timestamp)")
	comments = @(
		"String"
	)
	feedback = "@odata.type: microsoft.graph.alertFeedback"
	status = "@odata.type: microsoft.graph.alertStatus"
	tags = @(
		"String"
	)
	vendorInformation = @{
		provider = "String"
		vendor = "String"
	}
}

Update-MgBetaSecurityAlert -AlertId $alertId -BodyParameter $params

```
This example will request with prefer header


## PARAMETERS

### -ActivityGroupName
Name or alias of the activity group (attacker) this alert is attributed to.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AlertDetections

To construct, see NOTES section for ALERTDETECTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAlertDetection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AlertId
The unique identifier of alert

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AssignedTo
Name of the analyst the alert is assigned to for triage, investigation, or remediation (supports update).

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AzureSubscriptionId
Azure subscription ID, present if this alert is related to an Azure resource.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AzureTenantId
Microsoft Entra tenant ID.
Required.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Type: IMicrosoftGraphAlert
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Category
Category of the alert (for example, credentialTheft, ransomware).

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClosedDateTime
Time at which the alert was closed.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z (supports update).

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CloudAppStates
Security-related stateful information generated by the provider about the cloud application/s related to this alert.
To construct, see NOTES section for CLOUDAPPSTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphCloudAppSecurityState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Comments
Customer-provided comments on alert (for customer alert management) (supports update).

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confidence
Confidence of the detection logic (percentage between 1-100).

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -CreatedDateTime
Time at which the alert was created by the alert provider.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Required.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
Alert description.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DetectionIds
Set of alerts related to this alert entity (each alert is pushed to the SIEM as a separate record).

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EventDateTime
Time at which the event or events that served as the trigger to generate the alert occurred.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Required.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Feedback
alertFeedback

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FileStates
Security-related stateful information generated by the provider about the file(s) related to this alert.
To construct, see NOTES section for FILESTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphFileSecurityState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -HistoryStates
A collection of alertHistoryStates comprising an audit log of all updates made to an alert.
To construct, see NOTES section for HISTORYSTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAlertHistoryState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HostStates
Security-related stateful information generated by the provider about the host(s) related to this alert.
To construct, see NOTES section for HOSTSTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphHostSecurityState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The unique identifier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncidentIds
IDs of incidents related to current alert.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ISecurityIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InvestigationSecurityStates

To construct, see NOTES section for INVESTIGATIONSECURITYSTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphInvestigationSecurityState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastEventDateTime


```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
Time at which the alert entity was last modified.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MalwareStates
Threat Intelligence pertaining to malware related to this alert.
To construct, see NOTES section for MALWARESTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphMalwareState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MessageSecurityStates

To construct, see NOTES section for MESSAGESECURITYSTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphMessageSecurityState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkConnections
Security-related stateful information generated by the provider about the network connection(s) related to this alert.
To construct, see NOTES section for NETWORKCONNECTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphNetworkConnection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Processes
Security-related stateful information generated by the provider about the process or processes related to this alert.
To construct, see NOTES section for PROCESSES properties and create a hash table.

```yaml
Type: IMicrosoftGraphProcess[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RecommendedActions
Vendor/provider recommended action(s) to take as a result of the alert (for example, isolate machine, enforce2FA, reimage host).

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RegistryKeyStates
Security-related stateful information generated by the provider about the registry keys related to this alert.
To construct, see NOTES section for REGISTRYKEYSTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphRegistryKeyState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -SecurityResources
Resources related to current alert.
For example, for some alerts this can have the Azure Resource value.
To construct, see NOTES section for SECURITYRESOURCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityResource[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourceMaterials
Hyperlinks (URIs) to the source material related to the alert, for example, provider's user interface for alerts or log search.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tags
User-definable labels that can be applied to an alert and can serve as filter conditions (for example 'HVA', 'SAW') (supports update).

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Title
Alert title.
Required.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Triggers
Security-related information about the specific properties that triggered the alert (properties appearing in the alert).
Alerts might contain information about multiple users, hosts, files, ip addresses.
This field indicates which properties triggered the alert generation.
To construct, see NOTES section for TRIGGERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAlertTrigger[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UriClickSecurityStates

To construct, see NOTES section for URICLICKSECURITYSTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphUriClickSecurityState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserStates
Security-related stateful information generated by the provider about the user accounts related to this alert.
To construct, see NOTES section for USERSTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserSecurityState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VulnerabilityStates
Threat intelligence pertaining to one or more vulnerabilities related to this alert.
To construct, see NOTES section for VULNERABILITYSTATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphVulnerabilityState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAlert
### Microsoft.Graph.Beta.PowerShell.Models.ISecurityIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAlert
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ALERTDETECTIONS `<IMicrosoftGraphAlertDetection- `[]`>`: .
  - `[DetectionType <String>]`: 
  - `[Method <String>]`: 
  - `[Name <String>]`: 

BODYPARAMETER `<IMicrosoftGraphAlert>`: alert
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActivityGroupName <String>]`: Name or alias of the activity group (attacker) this alert is attributed to.
  - `[AlertDetections <IMicrosoftGraphAlertDetection- `[]`>]`: 
    - `[DetectionType <String>]`: 
    - `[Method <String>]`: 
    - `[Name <String>]`: 
  - `[AssignedTo <String>]`: Name of the analyst the alert is assigned to for triage, investigation, or remediation (supports update).
  - `[AzureSubscriptionId <String>]`: Azure subscription ID, present if this alert is related to an Azure resource.
  - `[AzureTenantId <String>]`: Microsoft Entra tenant ID.
Required.
  - `[Category <String>]`: Category of the alert (for example, credentialTheft, ransomware).
  - `[ClosedDateTime <DateTime?>]`: Time at which the alert was closed.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z (supports update).
  - `[CloudAppStates <IMicrosoftGraphCloudAppSecurityState- `[]`>]`: Security-related stateful information generated by the provider about the cloud application/s related to this alert.
    - `[DestinationServiceIP <String>]`: Destination IP Address of the connection to the cloud application/service.
    - `[DestinationServiceName <String>]`: Cloud application/service name (for example 'Salesforce', 'DropBox', etc.).
    - `[RiskScore <String>]`: Provider-generated/calculated risk score of the Cloud Application/Service.
Recommended value range of 0-1, which equates to a percentage.
  - `[Comments <String- `[]`>]`: Customer-provided comments on alert (for customer alert management) (supports update).
  - `[Confidence <Int32?>]`: Confidence of the detection logic (percentage between 1-100).
  - `[CreatedDateTime <DateTime?>]`: Time at which the alert was created by the alert provider.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Required.
  - `[Description <String>]`: Alert description.
  - `[DetectionIds <String- `[]`>]`: Set of alerts related to this alert entity (each alert is pushed to the SIEM as a separate record).
  - `[EventDateTime <DateTime?>]`: Time at which the event or events that served as the trigger to generate the alert occurred.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Required.
  - `[Feedback <String>]`: alertFeedback
  - `[FileStates <IMicrosoftGraphFileSecurityState- `[]`>]`: Security-related stateful information generated by the provider about the file(s) related to this alert.
    - `[FileHash <IMicrosoftGraphFileHash>]`: fileHash
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[HashType <String>]`: fileHashType
      - `[HashValue <String>]`: Value of the file hash.
    - `[Name <String>]`: File name (without path).
    - `[Path <String>]`: Full file path of the file/imageFile.
    - `[RiskScore <String>]`: Provider generated/calculated risk score of the alert file.
Recommended value range of 0-1, which equates to a percentage.
  - `[HistoryStates <IMicrosoftGraphAlertHistoryState- `[]`>]`: A collection of alertHistoryStates comprising an audit log of all updates made to an alert.
    - `[AppId <String>]`: The Application ID of the calling application that submitted an update (PATCH) to the alert.
The appId should be extracted from the auth token and not entered manually by the calling application.
    - `[AssignedTo <String>]`: UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).
    - `[Comments <String- `[]`>]`: Comment entered by signed-in user.
    - `[Feedback <String>]`: alertFeedback
    - `[Status <String>]`: alertStatus
    - `[UpdatedDateTime <DateTime?>]`: Date and time of the alert update.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[User <String>]`: UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).
  - `[HostStates <IMicrosoftGraphHostSecurityState- `[]`>]`: Security-related stateful information generated by the provider about the host(s) related to this alert.
    - `[Fqdn <String>]`: Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).
    - `[IsAzureAdJoined <Boolean?>]`: 
    - `[IsAzureAdRegistered <Boolean?>]`: 
    - `[IsHybridAzureDomainJoined <Boolean?>]`: True if the host is domain joined to an on-premises Active Directory domain.
    - `[NetBiosName <String>]`: The local host name, without the DNS domain name.
    - `[OS <String>]`: Host Operating System.
(For example, Windows 10, macOS, RHEL, etc.).
    - `[PrivateIPAddress <String>]`: Private (not routable) IPv4 or IPv6 address (see RFC 1918) at the time of the alert.
    - `[PublicIPAddress <String>]`: Publicly routable IPv4 or IPv6 address (see RFC 1918) at time of the alert.
    - `[RiskScore <String>]`: Provider-generated/calculated risk score of the host. 
Recommended value range of 0-1, which equates to a percentage.
  - `[IncidentIds <String- `[]`>]`: IDs of incidents related to current alert.
  - `[InvestigationSecurityStates <IMicrosoftGraphInvestigationSecurityState- `[]`>]`: 
    - `[Name <String>]`: 
    - `[Status <String>]`: 
  - `[LastEventDateTime <DateTime?>]`: 
  - `[LastModifiedDateTime <DateTime?>]`: Time at which the alert entity was last modified.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[MalwareStates <IMicrosoftGraphMalwareState- `[]`>]`: Threat Intelligence pertaining to malware related to this alert.
    - `[Category <String>]`: Provider-generated malware category (for example, trojan, ransomware, etc.).
    - `[Family <String>]`: Provider-generated malware family (for example, 'wannacry,' 'notpetya,' etc.).
    - `[Name <String>]`: Provider-generated malware variant name (for example, Trojan:Win32/Powessere.H).
    - `[Severity <String>]`: Provider-determined severity of this malware.
    - `[WasRunning <Boolean?>]`: Indicates whether the detected file (malware/vulnerability) was running at the time of detection or was detected at rest on the disk.
  - `[MessageSecurityStates <IMicrosoftGraphMessageSecurityState- `[]`>]`: 
    - `[ConnectingIP <String>]`: 
    - `[DeliveryAction <String>]`: 
    - `[DeliveryLocation <String>]`: 
    - `[Directionality <String>]`: 
    - `[InternetMessageId <String>]`: 
    - `[MessageFingerprint <String>]`: 
    - `[MessageReceivedDateTime <DateTime?>]`: 
    - `[MessageSubject <String>]`: 
    - `[NetworkMessageId <String>]`: 
  - `[NetworkConnections <IMicrosoftGraphNetworkConnection- `[]`>]`: Security-related stateful information generated by the provider about the network connection(s) related to this alert.
    - `[ApplicationName <String>]`: Name of the application managing the network connection (for example, Facebook, SMTP, etc.).
    - `[DestinationAddress <String>]`: Destination IP address (of the network connection).
    - `[DestinationDomain <String>]`: Destination domain portion of the destination URL.
(for example 'www.contoso.com').
    - `[DestinationLocation <String>]`: Location (by IP address mapping) associated with the destination of a network connection.
    - `[DestinationPort <String>]`: Destination port (of the network connection).
    - `[DestinationUrl <String>]`: Network connection URL/URI string - excluding parameters.
(for example 'www.contoso.com/products/default.html')
    - `[Direction <String>]`: connectionDirection
    - `[DomainRegisteredDateTime <DateTime?>]`: Date when the destination domain was registered.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[LocalDnsName <String>]`: The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).
    - `[NatDestinationAddress <String>]`: Network Address Translation destination IP address.
    - `[NatDestinationPort <String>]`: Network Address Translation destination port.
    - `[NatSourceAddress <String>]`: Network Address Translation source IP address.
    - `[NatSourcePort <String>]`: Network Address Translation source port.
    - `[Protocol <String>]`: securityNetworkProtocol
    - `[RiskScore <String>]`: Provider generated/calculated risk score of the network connection.
Recommended value range of 0-1, which equates to a percentage.
    - `[SourceAddress <String>]`: Source (i.e.
origin) IP address (of the network connection).
    - `[SourceLocation <String>]`: Location (by IP address mapping) associated with the source of a network connection.
    - `[SourcePort <String>]`: Source (i.e.
origin) IP port (of the network connection).
    - `[Status <String>]`: connectionStatus
    - `[UrlParameters <String>]`: Parameters (suffix) of the destination URL.
  - `[Processes <IMicrosoftGraphProcess- `[]`>]`: Security-related stateful information generated by the provider about the process or processes related to this alert.
    - `[AccountName <String>]`: User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.
    - `[CommandLine <String>]`: The full process invocation commandline including all parameters.
    - `[CreatedDateTime <DateTime?>]`: Time at which the process was started.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[FileHash <IMicrosoftGraphFileHash>]`: fileHash
    - `[IntegrityLevel <String>]`: processIntegrityLevel
    - `[IsElevated <Boolean?>]`: True if the process is elevated.
    - `[Name <String>]`: The name of the process' Image file.
    - `[ParentProcessCreatedDateTime <DateTime?>]`: DateTime at which the parent process was started.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[ParentProcessId <Int32?>]`: The Process ID (PID) of the parent process.
    - `[ParentProcessName <String>]`: The name of the image file of the parent process.
    - `[Path <String>]`: Full path, including filename.
    - `[ProcessId <Int32?>]`: The Process ID (PID) of the process.
  - `[RecommendedActions <String- `[]`>]`: Vendor/provider recommended action(s) to take as a result of the alert (for example, isolate machine, enforce2FA, reimage host).
  - `[RegistryKeyStates <IMicrosoftGraphRegistryKeyState- `[]`>]`: Security-related stateful information generated by the provider about the registry keys related to this alert.
    - `[Hive <String>]`: registryHive
    - `[Key <String>]`: Current (i.e.
changed) registry key (excludes HIVE).
    - `[OldKey <String>]`: Previous (i.e.
before changed) registry key (excludes HIVE).
    - `[OldValueData <String>]`: Previous (i.e.
before changed) registry key value data (contents).
    - `[OldValueName <String>]`: Previous (i.e.
before changed) registry key value name.
    - `[Operation <String>]`: registryOperation
    - `[ProcessId <Int32?>]`: Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).
    - `[ValueData <String>]`: Current (i.e.
changed) registry key value data (contents).
    - `[ValueName <String>]`: Current (i.e.
changed) registry key value name
    - `[ValueType <String>]`: registryValueType
  - `[SecurityResources <IMicrosoftGraphSecurityResource- `[]`>]`: Resources related to current alert.
For example, for some alerts this can have the Azure Resource value.
    - `[Resource <String>]`: Name of the resource that is related to current alert.
Required.
    - `[ResourceType <String>]`: securityResourceType
  - `[Severity <String>]`: alertSeverity
  - `[SourceMaterials <String- `[]`>]`: Hyperlinks (URIs) to the source material related to the alert, for example, provider's user interface for alerts or log search.
  - `[Status <String>]`: alertStatus
  - `[Tags <String- `[]`>]`: User-definable labels that can be applied to an alert and can serve as filter conditions (for example 'HVA', 'SAW') (supports update).
  - `[Title <String>]`: Alert title.
Required.
  - `[Triggers <IMicrosoftGraphAlertTrigger- `[]`>]`: Security-related information about the specific properties that triggered the alert (properties appearing in the alert).
Alerts might contain information about multiple users, hosts, files, ip addresses.
This field indicates which properties triggered the alert generation.
    - `[Name <String>]`: Name of the property serving as a detection trigger.
    - `[Type <String>]`: Type of the property in the key:value pair for interpretation.
For example, String, Boolean etc.
    - `[Value <String>]`: Value of the property serving as a detection trigger.
  - `[UriClickSecurityStates <IMicrosoftGraphUriClickSecurityState- `[]`>]`: 
    - `[ClickAction <String>]`: 
    - `[ClickDateTime <DateTime?>]`: 
    - `[Id <String>]`: 
    - `[SourceId <String>]`: 
    - `[UriDomain <String>]`: 
    - `[Verdict <String>]`: 
  - `[UserStates <IMicrosoftGraphUserSecurityState- `[]`>]`: Security-related stateful information generated by the provider about the user accounts related to this alert.
    - `[AadUserId <String>]`: AAD User object identifier (GUID) - represents the physical/multi-account user entity.
    - `[AccountName <String>]`: Account name of user account (without Active Directory domain or DNS domain) - (also called mailNickName).
    - `[DomainName <String>]`: NetBIOS/Active Directory domain of user account (that is, domain/account format).
    - `[EmailRole <String>]`: emailRole
    - `[IsVpn <Boolean?>]`: Indicates whether the user logged on through a VPN.
    - `[LogonDateTime <DateTime?>]`: Time at which the sign-in occurred.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[LogonIP <String>]`: IP Address the sign-in request originated from.
    - `[LogonId <String>]`: User sign-in ID.
    - `[LogonLocation <String>]`: Location (by IP address mapping) associated with a user sign-in event by this user.
    - `[LogonType <String>]`: logonType
    - `[OnPremisesSecurityIdentifier <String>]`: Active Directory (on-premises) Security Identifier (SID) of the user.
    - `[RiskScore <String>]`: Provider-generated/calculated risk score of the user account.
Recommended value range of 0-1, which equates to a percentage.
    - `[UserAccountType <String>]`: userAccountSecurityType
    - `[UserPrincipalName <String>]`: User sign-in name - internet format: (user account name)@(user account DNS domain name).
  - `[VendorInformation <IMicrosoftGraphSecurityVendorInformation>]`: securityVendorInformation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Provider <String>]`: Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.
    - `[ProviderVersion <String>]`: Version of the provider or subprovider, if it exists, that generated the alert.
Required
    - `[SubProvider <String>]`: Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.
    - `[Vendor <String>]`: Name of the alert vendor (for example, Microsoft, Dell, FireEye).
Required
  - `[VulnerabilityStates <IMicrosoftGraphVulnerabilityState- `[]`>]`: Threat intelligence pertaining to one or more vulnerabilities related to this alert.
    - `[Cve <String>]`: Common Vulnerabilities and Exposures (CVE) for the vulnerability.
    - `[Severity <String>]`: Base Common Vulnerability Scoring System (CVSS) severity score for this vulnerability.
    - `[WasRunning <Boolean?>]`: Indicates whether the detected vulnerability (file) was running at the time of detection or was the file detected at rest on the disk.

CLOUDAPPSTATES `<IMicrosoftGraphCloudAppSecurityState- `[]`>`: Security-related stateful information generated by the provider about the cloud application/s related to this alert.
  - `[DestinationServiceIP <String>]`: Destination IP Address of the connection to the cloud application/service.
  - `[DestinationServiceName <String>]`: Cloud application/service name (for example 'Salesforce', 'DropBox', etc.).
  - `[RiskScore <String>]`: Provider-generated/calculated risk score of the Cloud Application/Service.
Recommended value range of 0-1, which equates to a percentage.

FILESTATES `<IMicrosoftGraphFileSecurityState- `[]`>`: Security-related stateful information generated by the provider about the file(s) related to this alert.
  - `[FileHash <IMicrosoftGraphFileHash>]`: fileHash
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[HashType <String>]`: fileHashType
    - `[HashValue <String>]`: Value of the file hash.
  - `[Name <String>]`: File name (without path).
  - `[Path <String>]`: Full file path of the file/imageFile.
  - `[RiskScore <String>]`: Provider generated/calculated risk score of the alert file.
Recommended value range of 0-1, which equates to a percentage.

HISTORYSTATES `<IMicrosoftGraphAlertHistoryState- `[]`>`: A collection of alertHistoryStates comprising an audit log of all updates made to an alert.
  - `[AppId <String>]`: The Application ID of the calling application that submitted an update (PATCH) to the alert.
The appId should be extracted from the auth token and not entered manually by the calling application.
  - `[AssignedTo <String>]`: UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).
  - `[Comments <String- `[]`>]`: Comment entered by signed-in user.
  - `[Feedback <String>]`: alertFeedback
  - `[Status <String>]`: alertStatus
  - `[UpdatedDateTime <DateTime?>]`: Date and time of the alert update.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[User <String>]`: UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).

HOSTSTATES `<IMicrosoftGraphHostSecurityState- `[]`>`: Security-related stateful information generated by the provider about the host(s) related to this alert.
  - `[Fqdn <String>]`: Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).
  - `[IsAzureAdJoined <Boolean?>]`: 
  - `[IsAzureAdRegistered <Boolean?>]`: 
  - `[IsHybridAzureDomainJoined <Boolean?>]`: True if the host is domain joined to an on-premises Active Directory domain.
  - `[NetBiosName <String>]`: The local host name, without the DNS domain name.
  - `[OS <String>]`: Host Operating System.
(For example, Windows 10, macOS, RHEL, etc.).
  - `[PrivateIPAddress <String>]`: Private (not routable) IPv4 or IPv6 address (see RFC 1918) at the time of the alert.
  - `[PublicIPAddress <String>]`: Publicly routable IPv4 or IPv6 address (see RFC 1918) at time of the alert.
  - `[RiskScore <String>]`: Provider-generated/calculated risk score of the host. 
Recommended value range of 0-1, which equates to a percentage.

INPUTOBJECT `<ISecurityIdentity>`: Identity Parameter
  - `[AlertId <String>]`: The unique identifier of alert
  - `[AnalyzedEmailId <String>]`: The unique identifier of analyzedEmail
  - `[ArticleId <String>]`: The unique identifier of article
  - `[ArticleIndicatorId <String>]`: The unique identifier of articleIndicator
  - `[AttackSimulationOperationId <String>]`: The unique identifier of attackSimulationOperation
  - `[AuditLogQueryId <String>]`: The unique identifier of auditLogQuery
  - `[AuditLogRecordId <String>]`: The unique identifier of auditLogRecord
  - `[AuthoredNoteId <String>]`: The unique identifier of authoredNote
  - `[AuthorityTemplateId <String>]`: The unique identifier of authorityTemplate
  - `[CaseOperationId <String>]`: The unique identifier of caseOperation
  - `[CategoryTemplateId <String>]`: The unique identifier of categoryTemplate
  - `[CitationTemplateId <String>]`: The unique identifier of citationTemplate
  - `[CloudAppDiscoveryReportId <String>]`: The unique identifier of cloudAppDiscoveryReport
  - `[CloudAppSecurityProfileId <String>]`: The unique identifier of cloudAppSecurityProfile
  - `[CustomerInsightTenantId <String>]`: The unique identifier of customerInsight
  - `[DataSourceId <String>]`: The unique identifier of dataSource
  - `[DepartmentTemplateId <String>]`: The unique identifier of departmentTemplate
  - `[DetectionRuleId <String>]`: The unique identifier of detectionRule
  - `[DispositionReviewStageNumber <String>]`: The unique identifier of dispositionReviewStage
  - `[DomainSecurityProfileId <String>]`: The unique identifier of domainSecurityProfile
  - `[EdiscoveryCaseId <String>]`: The unique identifier of ediscoveryCase
  - `[EdiscoveryCaseMemberId <String>]`: The unique identifier of ediscoveryCaseMember
  - `[EdiscoveryCustodianId <String>]`: The unique identifier of ediscoveryCustodian
  - `[EdiscoveryFileId <String>]`: The unique identifier of ediscoveryFile
  - `[EdiscoveryHoldPolicyId <String>]`: The unique identifier of ediscoveryHoldPolicy
  - `[EdiscoveryNoncustodialDataSourceId <String>]`: The unique identifier of ediscoveryNoncustodialDataSource
  - `[EdiscoveryReviewSetId <String>]`: The unique identifier of ediscoveryReviewSet
  - `[EdiscoveryReviewSetQueryId <String>]`: The unique identifier of ediscoveryReviewSetQuery
  - `[EdiscoveryReviewTagId <String>]`: The unique identifier of ediscoveryReviewTag
  - `[EdiscoveryReviewTagId1 <String>]`: The unique identifier of ediscoveryReviewTag
  - `[EdiscoverySearchId <String>]`: The unique identifier of ediscoverySearch
  - `[EmailThreatSubmissionId <String>]`: The unique identifier of emailThreatSubmission
  - `[EmailThreatSubmissionPolicyId <String>]`: The unique identifier of emailThreatSubmissionPolicy
  - `[EndUserNotificationDetailId <String>]`: The unique identifier of endUserNotificationDetail
  - `[EndUserNotificationId <String>]`: The unique identifier of endUserNotification
  - `[FilePlanReferenceTemplateId <String>]`: The unique identifier of filePlanReferenceTemplate
  - `[FileSecurityProfileId <String>]`: The unique identifier of fileSecurityProfile
  - `[FileThreatSubmissionId <String>]`: The unique identifier of fileThreatSubmission
  - `[HealthIssueId <String>]`: The unique identifier of healthIssue
  - `[HostComponentId <String>]`: The unique identifier of hostComponent
  - `[HostCookieId <String>]`: The unique identifier of hostCookie
  - `[HostId <String>]`: The unique identifier of host
  - `[HostPairId <String>]`: The unique identifier of hostPair
  - `[HostPortId <String>]`: The unique identifier of hostPort
  - `[HostSecurityProfileId <String>]`: The unique identifier of hostSecurityProfile
  - `[HostSslCertificateId <String>]`: The unique identifier of hostSslCertificate
  - `[HostTrackerId <String>]`: The unique identifier of hostTracker
  - `[IPSecurityProfileId <String>]`: The unique identifier of ipSecurityProfile
  - `[IncidentId <String>]`: The unique identifier of incident
  - `[IntelligenceProfileId <String>]`: The unique identifier of intelligenceProfile
  - `[IntelligenceProfileIndicatorId <String>]`: The unique identifier of intelligenceProfileIndicator
  - `[LandingPageDetailId <String>]`: The unique identifier of landingPageDetail
  - `[LandingPageId <String>]`: The unique identifier of landingPage
  - `[LoginPageId <String>]`: The unique identifier of loginPage
  - `[PartnerSecurityAlertId <String>]`: The unique identifier of partnerSecurityAlert
  - `[PassiveDnsRecordId <String>]`: The unique identifier of passiveDnsRecord
  - `[PayloadId <String>]`: The unique identifier of payload
  - `[ProviderTenantSettingId <String>]`: The unique identifier of providerTenantSetting
  - `[RetentionEventId <String>]`: The unique identifier of retentionEvent
  - `[RetentionEventTypeId <String>]`: The unique identifier of retentionEventType
  - `[RetentionLabelId <String>]`: The unique identifier of retentionLabel
  - `[SecureScoreControlProfileId <String>]`: The unique identifier of secureScoreControlProfile
  - `[SecureScoreId <String>]`: The unique identifier of secureScore
  - `[SecurityActionId <String>]`: The unique identifier of securityAction
  - `[SecurityRequirementId <String>]`: The unique identifier of securityRequirement
  - `[SecurityScoreHistoryId <String>]`: The unique identifier of securityScoreHistory
  - `[SensitivityLabelId <String>]`: The unique identifier of sensitivityLabel
  - `[SensorId <String>]`: The unique identifier of sensor
  - `[SimulationAutomationId <String>]`: The unique identifier of simulationAutomation
  - `[SimulationAutomationRunId <String>]`: The unique identifier of simulationAutomationRun
  - `[SimulationId <String>]`: The unique identifier of simulation
  - `[SiteSourceId <String>]`: The unique identifier of siteSource
  - `[SslCertificateId <String>]`: The unique identifier of sslCertificate
  - `[SubcategoryTemplateId <String>]`: The unique identifier of subcategoryTemplate
  - `[SubdomainId <String>]`: The unique identifier of subdomain
  - `[SubjectRightsRequestId <String>]`: The unique identifier of subjectRightsRequest
  - `[TiIndicatorId <String>]`: The unique identifier of tiIndicator
  - `[TrainingCampaignId <String>]`: The unique identifier of trainingCampaign
  - `[TrainingId <String>]`: The unique identifier of training
  - `[TrainingLanguageDetailId <String>]`: The unique identifier of trainingLanguageDetail
  - `[UnifiedGroupSourceId <String>]`: The unique identifier of unifiedGroupSource
  - `[UrlThreatSubmissionId <String>]`: The unique identifier of urlThreatSubmission
  - `[UserId <String>]`: The unique identifier of user
  - `[UserPrincipalName <String>]`: Alternate key of user
  - `[UserSecurityProfileId <String>]`: The unique identifier of userSecurityProfile
  - `[UserSourceId <String>]`: The unique identifier of userSource
  - `[VulnerabilityComponentId <String>]`: The unique identifier of vulnerabilityComponent
  - `[VulnerabilityId <String>]`: The unique identifier of vulnerability
  - `[WhoisHistoryRecordId <String>]`: The unique identifier of whoisHistoryRecord
  - `[WhoisRecordId <String>]`: The unique identifier of whoisRecord

INVESTIGATIONSECURITYSTATES `<IMicrosoftGraphInvestigationSecurityState- `[]`>`: .
  - `[Name <String>]`: 
  - `[Status <String>]`: 

MALWARESTATES `<IMicrosoftGraphMalwareState- `[]`>`: Threat Intelligence pertaining to malware related to this alert.
  - `[Category <String>]`: Provider-generated malware category (for example, trojan, ransomware, etc.).
  - `[Family <String>]`: Provider-generated malware family (for example, 'wannacry,' 'notpetya,' etc.).
  - `[Name <String>]`: Provider-generated malware variant name (for example, Trojan:Win32/Powessere.H).
  - `[Severity <String>]`: Provider-determined severity of this malware.
  - `[WasRunning <Boolean?>]`: Indicates whether the detected file (malware/vulnerability) was running at the time of detection or was detected at rest on the disk.

MESSAGESECURITYSTATES `<IMicrosoftGraphMessageSecurityState- `[]`>`: .
  - `[ConnectingIP <String>]`: 
  - `[DeliveryAction <String>]`: 
  - `[DeliveryLocation <String>]`: 
  - `[Directionality <String>]`: 
  - `[InternetMessageId <String>]`: 
  - `[MessageFingerprint <String>]`: 
  - `[MessageReceivedDateTime <DateTime?>]`: 
  - `[MessageSubject <String>]`: 
  - `[NetworkMessageId <String>]`: 

NETWORKCONNECTIONS `<IMicrosoftGraphNetworkConnection- `[]`>`: Security-related stateful information generated by the provider about the network connection(s) related to this alert.
  - `[ApplicationName <String>]`: Name of the application managing the network connection (for example, Facebook, SMTP, etc.).
  - `[DestinationAddress <String>]`: Destination IP address (of the network connection).
  - `[DestinationDomain <String>]`: Destination domain portion of the destination URL.
(for example 'www.contoso.com').
  - `[DestinationLocation <String>]`: Location (by IP address mapping) associated with the destination of a network connection.
  - `[DestinationPort <String>]`: Destination port (of the network connection).
  - `[DestinationUrl <String>]`: Network connection URL/URI string - excluding parameters.
(for example 'www.contoso.com/products/default.html')
  - `[Direction <String>]`: connectionDirection
  - `[DomainRegisteredDateTime <DateTime?>]`: Date when the destination domain was registered.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[LocalDnsName <String>]`: The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).
  - `[NatDestinationAddress <String>]`: Network Address Translation destination IP address.
  - `[NatDestinationPort <String>]`: Network Address Translation destination port.
  - `[NatSourceAddress <String>]`: Network Address Translation source IP address.
  - `[NatSourcePort <String>]`: Network Address Translation source port.
  - `[Protocol <String>]`: securityNetworkProtocol
  - `[RiskScore <String>]`: Provider generated/calculated risk score of the network connection.
Recommended value range of 0-1, which equates to a percentage.
  - `[SourceAddress <String>]`: Source (i.e.
origin) IP address (of the network connection).
  - `[SourceLocation <String>]`: Location (by IP address mapping) associated with the source of a network connection.
  - `[SourcePort <String>]`: Source (i.e.
origin) IP port (of the network connection).
  - `[Status <String>]`: connectionStatus
  - `[UrlParameters <String>]`: Parameters (suffix) of the destination URL.

PROCESSES `<IMicrosoftGraphProcess- `[]`>`: Security-related stateful information generated by the provider about the process or processes related to this alert.
  - `[AccountName <String>]`: User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.
  - `[CommandLine <String>]`: The full process invocation commandline including all parameters.
  - `[CreatedDateTime <DateTime?>]`: Time at which the process was started.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[FileHash <IMicrosoftGraphFileHash>]`: fileHash
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[HashType <String>]`: fileHashType
    - `[HashValue <String>]`: Value of the file hash.
  - `[IntegrityLevel <String>]`: processIntegrityLevel
  - `[IsElevated <Boolean?>]`: True if the process is elevated.
  - `[Name <String>]`: The name of the process' Image file.
  - `[ParentProcessCreatedDateTime <DateTime?>]`: DateTime at which the parent process was started.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[ParentProcessId <Int32?>]`: The Process ID (PID) of the parent process.
  - `[ParentProcessName <String>]`: The name of the image file of the parent process.
  - `[Path <String>]`: Full path, including filename.
  - `[ProcessId <Int32?>]`: The Process ID (PID) of the process.

REGISTRYKEYSTATES `<IMicrosoftGraphRegistryKeyState- `[]`>`: Security-related stateful information generated by the provider about the registry keys related to this alert.
  - `[Hive <String>]`: registryHive
  - `[Key <String>]`: Current (i.e.
changed) registry key (excludes HIVE).
  - `[OldKey <String>]`: Previous (i.e.
before changed) registry key (excludes HIVE).
  - `[OldValueData <String>]`: Previous (i.e.
before changed) registry key value data (contents).
  - `[OldValueName <String>]`: Previous (i.e.
before changed) registry key value name.
  - `[Operation <String>]`: registryOperation
  - `[ProcessId <Int32?>]`: Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).
  - `[ValueData <String>]`: Current (i.e.
changed) registry key value data (contents).
  - `[ValueName <String>]`: Current (i.e.
changed) registry key value name
  - `[ValueType <String>]`: registryValueType

SECURITYRESOURCES `<IMicrosoftGraphSecurityResource- `[]`>`: Resources related to current alert.
For example, for some alerts this can have the Azure Resource value.
  - `[Resource <String>]`: Name of the resource that is related to current alert.
Required.
  - `[ResourceType <String>]`: securityResourceType

TRIGGERS `<IMicrosoftGraphAlertTrigger- `[]`>`: Security-related information about the specific properties that triggered the alert (properties appearing in the alert).
Alerts might contain information about multiple users, hosts, files, ip addresses.
This field indicates which properties triggered the alert generation.
  - `[Name <String>]`: Name of the property serving as a detection trigger.
  - `[Type <String>]`: Type of the property in the key:value pair for interpretation.
For example, String, Boolean etc.
  - `[Value <String>]`: Value of the property serving as a detection trigger.

URICLICKSECURITYSTATES `<IMicrosoftGraphUriClickSecurityState- `[]`>`: .
  - `[ClickAction <String>]`: 
  - `[ClickDateTime <DateTime?>]`: 
  - `[Id <String>]`: 
  - `[SourceId <String>]`: 
  - `[UriDomain <String>]`: 
  - `[Verdict <String>]`: 

USERSTATES `<IMicrosoftGraphUserSecurityState- `[]`>`: Security-related stateful information generated by the provider about the user accounts related to this alert.
  - `[AadUserId <String>]`: AAD User object identifier (GUID) - represents the physical/multi-account user entity.
  - `[AccountName <String>]`: Account name of user account (without Active Directory domain or DNS domain) - (also called mailNickName).
  - `[DomainName <String>]`: NetBIOS/Active Directory domain of user account (that is, domain/account format).
  - `[EmailRole <String>]`: emailRole
  - `[IsVpn <Boolean?>]`: Indicates whether the user logged on through a VPN.
  - `[LogonDateTime <DateTime?>]`: Time at which the sign-in occurred.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[LogonIP <String>]`: IP Address the sign-in request originated from.
  - `[LogonId <String>]`: User sign-in ID.
  - `[LogonLocation <String>]`: Location (by IP address mapping) associated with a user sign-in event by this user.
  - `[LogonType <String>]`: logonType
  - `[OnPremisesSecurityIdentifier <String>]`: Active Directory (on-premises) Security Identifier (SID) of the user.
  - `[RiskScore <String>]`: Provider-generated/calculated risk score of the user account.
Recommended value range of 0-1, which equates to a percentage.
  - `[UserAccountType <String>]`: userAccountSecurityType
  - `[UserPrincipalName <String>]`: User sign-in name - internet format: (user account name)@(user account DNS domain name).

VENDORINFORMATION `<IMicrosoftGraphSecurityVendorInformation>`: securityVendorInformation
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Provider <String>]`: Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.
  - `[ProviderVersion <String>]`: Version of the provider or subprovider, if it exists, that generated the alert.
Required
  - `[SubProvider <String>]`: Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.
  - `[Vendor <String>]`: Name of the alert vendor (for example, Microsoft, Dell, FireEye).
Required

VULNERABILITYSTATES `<IMicrosoftGraphVulnerabilityState- `[]`>`: Threat intelligence pertaining to one or more vulnerabilities related to this alert.
  - `[Cve <String>]`: Common Vulnerabilities and Exposures (CVE) for the vulnerability.
  - `[Severity <String>]`: Base Common Vulnerability Scoring System (CVSS) severity score for this vulnerability.
  - `[WasRunning <Boolean?>]`: Indicates whether the detected vulnerability (file) was running at the time of detection or was the file detected at rest on the disk.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/update-mgbetasecurityalert](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/update-mgbetasecurityalert)

[https://learn.microsoft.com/graph/api/alert-update?view=graph-rest-beta](https://learn.microsoft.com/graph/api/alert-update?view=graph-rest-beta)























