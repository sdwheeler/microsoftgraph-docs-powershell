---
external help file: Microsoft.Graph.Beta.Reports-help.xml
Module Name: Microsoft.Graph.Beta.Reports
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/get-mgbetareportserviceactivityactiveusermetricforoutlookmobilebyreademail
schema: 2.0.0
ms.subservice: m365-monitoring-service
---

# Get-MgBetaReportServiceActivityActiveUserMetricForOutlookMobileByReadEmail

## SYNOPSIS
Get all the active usage based on the number of users who successfully read emails using Outlook apps for mobile.

## SYNTAX

### Get (Default)
```
Get-MgBetaReportServiceActivityActiveUserMetricForOutlookMobileByReadEmail
 -ExclusiveIntervalEndDateTime <DateTime> -InclusiveIntervalStartDateTime <DateTime>
 [-AggregationIntervalInMinutes <Int32>] [-Count] [-Filter <String>] [-Search <String>] [-Skip <Int32>]
 [-Top <Int32>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaReportServiceActivityActiveUserMetricForOutlookMobileByReadEmail -InputObject <IReportsIdentity>
 [-AggregationIntervalInMinutes <Int32>] [-Count] [-Filter <String>] [-Search <String>] [-Skip <Int32>]
 [-Top <Int32>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Get all the active usage based on the number of users who successfully read emails using Outlook apps for mobile.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Reports

Get-MgBetaReportServiceActivityActiveUserMetricForOutlookMobileByReadEmail

```
This example shows how to use the Get-MgBetaReportServiceActivityActiveUserMetricForOutlookMobileByReadEmail Cmdlet.


## PARAMETERS

### -AggregationIntervalInMinutes
Usage: aggregationIntervalInMinutes=@aggregationIntervalInMinutes

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

### -ExclusiveIntervalEndDateTime
Usage: exclusiveIntervalEndDateTime={exclusiveIntervalEndDateTime}

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

### -InclusiveIntervalStartDateTime
Usage: inclusiveIntervalStartDateTime={inclusiveIntervalStartDateTime}

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IReportsIdentity
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

### Microsoft.Graph.Beta.PowerShell.Models.IReportsIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphServiceActivityValueMetric
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IReportsIdentity>`: Identity Parameter
  - `[ActiveUsersMetricId <String>]`: The unique identifier of activeUsersMetric
  - `[AlertConfigurationId <String>]`: The unique identifier of alertConfiguration
  - `[AlertId <String>]`: The unique identifier of alert
  - `[AppCredentialSignInActivityId <String>]`: The unique identifier of appCredentialSignInActivity
  - `[ApplicationSignInDetailedSummaryId <String>]`: The unique identifier of applicationSignInDetailedSummary
  - `[AuthenticationsMetricId <String>]`: The unique identifier of authenticationsMetric
  - `[CredentialUserRegistrationDetailsId <String>]`: The unique identifier of credentialUserRegistrationDetails
  - `[CustomSecurityAttributeAuditId <String>]`: The unique identifier of customSecurityAttributeAudit
  - `[DailyInactiveUsersByApplicationMetricId <String>]`: The unique identifier of dailyInactiveUsersByApplicationMetric
  - `[DailyInactiveUsersMetricId <String>]`: The unique identifier of dailyInactiveUsersMetric
  - `[Date <DateTime?>]`: Usage: date={date}
  - `[DeviceManagementCachedReportConfigurationId <String>]`: The unique identifier of deviceManagementCachedReportConfiguration
  - `[DeviceManagementExportJobId <String>]`: The unique identifier of deviceManagementExportJob
  - `[DirectoryAuditId <String>]`: The unique identifier of directoryAudit
  - `[EndDateTime <DateTime?>]`: Usage: endDateTime={endDateTime}
  - `[ExclusiveIntervalEndDateTime <DateTime?>]`: Usage: exclusiveIntervalEndDateTime={exclusiveIntervalEndDateTime}
  - `[Filter <String>]`: Usage: filter='{filter}'
  - `[GroupId <String>]`: Usage: groupId='{groupId}'
  - `[IncludedUserRoles <String>]`: Usage: includedUserRoles='{includedUserRoles}'
  - `[IncludedUserTypes <String>]`: Usage: includedUserTypes='{includedUserTypes}'
  - `[InclusiveIntervalStartDateTime <DateTime?>]`: Usage: inclusiveIntervalStartDateTime={inclusiveIntervalStartDateTime}
  - `[InsightSummaryId <String>]`: The unique identifier of insightSummary
  - `[ManifestId <String>]`: The unique identifier of manifest
  - `[MfaCompletionMetricId <String>]`: The unique identifier of mfaCompletionMetric
  - `[MfaTelecomFraudMetricId <String>]`: The unique identifier of mfaTelecomFraudMetric
  - `[MfaUserCountMetricId <String>]`: The unique identifier of mfaUserCountMetric
  - `[MonthlyInactiveUsersByApplicationMetricId <String>]`: The unique identifier of monthlyInactiveUsersByApplicationMetric
  - `[MonthlyInactiveUsersMetricId <String>]`: The unique identifier of monthlyInactiveUsersMetric
  - `[OperationId <String>]`: The unique identifier of operation
  - `[Period <String>]`: Usage: period='{period}'
  - `[PrintUsageByPrinterId <String>]`: The unique identifier of printUsageByPrinter
  - `[PrintUsageByUserId <String>]`: The unique identifier of printUsageByUser
  - `[PrintUsageId <String>]`: The unique identifier of printUsage
  - `[PrinterId <String>]`: Usage: printerId='{printerId}'
  - `[ProvisioningObjectSummaryId <String>]`: The unique identifier of provisioningObjectSummary
  - `[SelfServiceSignUpId <String>]`: The unique identifier of selfServiceSignUp
  - `[ServicePrincipalSignInActivityId <String>]`: The unique identifier of servicePrincipalSignInActivity
  - `[SignInId <String>]`: The unique identifier of signIn
  - `[Skip <Int32?>]`: Usage: skip={skip}
  - `[SkipToken <String>]`: Usage: skipToken='{skipToken}'
  - `[StartDateTime <DateTime?>]`: Usage: startDateTime={startDateTime}
  - `[Top <Int32?>]`: Usage: top={top}
  - `[UserCountMetricId <String>]`: The unique identifier of userCountMetric
  - `[UserCredentialUsageDetailsId <String>]`: The unique identifier of userCredentialUsageDetails
  - `[UserId <String>]`: Usage: userId='{userId}'
  - `[UserRegistrationDetailsId <String>]`: The unique identifier of userRegistrationDetails
  - `[UserRequestsMetricId <String>]`: The unique identifier of userRequestsMetric
  - `[UserSignUpMetricId <String>]`: The unique identifier of userSignUpMetric

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/get-mgbetareportserviceactivityactiveusermetricforoutlookmobilebyreademail](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/get-mgbetareportserviceactivityactiveusermetricforoutlookmobilebyreademail)

[https://learn.microsoft.com/graph/api/serviceactivity-getactiveusermetricsforoutlookmobilebyreademail?view=graph-rest-beta](https://learn.microsoft.com/graph/api/serviceactivity-getactiveusermetricsforoutlookmobilebyreademail?view=graph-rest-beta)























