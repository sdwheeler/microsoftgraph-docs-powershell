---
external help file: Microsoft.Graph.Beta.NetworkAccess-help.xml
Module Name: Microsoft.Graph.Beta.NetworkAccess
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.networkaccess/get-mgbetanetworkaccessreportdeviceusagesummary
schema: 2.0.0
---

# Get-MgBetaNetworkAccessReportDeviceUsageSummary

## SYNOPSIS
Get a summary of device onboarding and offboarding within a specified timeframe.
This summary includes the total number of devices, active devices, and inactive devices.

## SYNTAX

### Get (Default)
```
Get-MgBetaNetworkAccessReportDeviceUsageSummary -ActivityPivotDateTime <DateTime> -EndDateTime <DateTime>
 -StartDateTime <DateTime> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaNetworkAccessReportDeviceUsageSummary -InputObject <INetworkAccessIdentity>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Get a summary of device onboarding and offboarding within a specified timeframe.
This summary includes the total number of devices, active devices, and inactive devices.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | NetworkAccess-Reports.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | NetworkAccess-Reports.Read.All,  |

## EXAMPLES

## PARAMETERS

### -ActivityPivotDateTime
Usage: activityPivotDateTime={activityPivotDateTime}

```yaml
Type: DateTime
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndDateTime
Usage: endDateTime={endDateTime}

```yaml
Type: DateTime
Parameter Sets: Get
Aliases:

Required: True
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: INetworkAccessIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
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

### -StartDateTime
Usage: startDateTime={startDateTime}

```yaml
Type: DateTime
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.INetworkAccessIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphNetworkaccessDeviceUsageSummary
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<INetworkAccessIdentity>`: Identity Parameter
  - `[ActivityPivotDateTime <DateTime?>]`: Usage: activityPivotDateTime={activityPivotDateTime}
  - `[AggregatedBy <String>]`: Usage: aggregatedBy='{aggregatedBy}'
  - `[AlertId <String>]`: The unique identifier of alert
  - `[BranchSiteId <String>]`: The unique identifier of branchSite
  - `[ConditionalAccessPolicyId <String>]`: The unique identifier of conditionalAccessPolicy
  - `[ConnectivityConfigurationLinkId <String>]`: The unique identifier of connectivityConfigurationLink
  - `[DeviceLinkId <String>]`: The unique identifier of deviceLink
  - `[DiscoveryPivotDateTime <DateTime?>]`: Usage: discoveryPivotDateTime={discoveryPivotDateTime}
  - `[EndDateTime <DateTime?>]`: Usage: endDateTime={endDateTime}
  - `[FilteringPolicyId <String>]`: The unique identifier of filteringPolicy
  - `[FilteringProfileId <String>]`: The unique identifier of filteringProfile
  - `[ForwardingPolicyId <String>]`: The unique identifier of forwardingPolicy
  - `[ForwardingProfileId <String>]`: The unique identifier of forwardingProfile
  - `[NetworkAccessTrafficTransactionId <String>]`: The unique identifier of networkAccessTraffic
  - `[PolicyLinkId <String>]`: The unique identifier of policyLink
  - `[PolicyRuleId <String>]`: The unique identifier of policyRule
  - `[RemoteNetworkHealthEventId <String>]`: The unique identifier of remoteNetworkHealthEvent
  - `[RemoteNetworkId <String>]`: The unique identifier of remoteNetwork
  - `[StartDateTime <DateTime?>]`: Usage: startDateTime={startDateTime}

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.networkaccess/get-mgbetanetworkaccessreportdeviceusagesummary](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.networkaccess/get-mgbetanetworkaccessreportdeviceusagesummary)
























