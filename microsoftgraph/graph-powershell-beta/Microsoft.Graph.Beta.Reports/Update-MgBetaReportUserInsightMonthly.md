---
external help file: Microsoft.Graph.Beta.Reports-help.xml
Module Name: Microsoft.Graph.Beta.Reports
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/update-mgbetareportuserinsightmonthly
schema: 2.0.0
---

# Update-MgBetaReportUserInsightMonthly

## SYNOPSIS
Update the navigation property monthly in reports

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaReportUserInsightMonthly [-ResponseHeadersVariable <String>]
 [-ActiveUsers <IMicrosoftGraphActiveUsersMetric[]>] [-AdditionalProperties <Hashtable>]
 [-Authentications <IMicrosoftGraphAuthenticationsMetric[]>] [-Id <String>]
 [-InactiveUsers <IMicrosoftGraphMonthlyInactiveUsersMetric[]>]
 [-InactiveUsersByApplication <IMicrosoftGraphMonthlyInactiveUsersByApplicationMetric[]>]
 [-MfaCompletions <IMicrosoftGraphMfaCompletionMetric[]>]
 [-MfaRegisteredUsers <IMicrosoftGraphMfaUserCountMetric[]>] [-Requests <IMicrosoftGraphUserRequestsMetric[]>]
 [-SignUps <IMicrosoftGraphUserSignUpMetric[]>] [-Summary <IMicrosoftGraphInsightSummary[]>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaReportUserInsightMonthly -BodyParameter <IMicrosoftGraphMonthlyUserInsightMetricsRoot>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property monthly in reports

## EXAMPLES

## PARAMETERS

### -ActiveUsers
Insights for active users on apps registered in the tenant for a specified period.
To construct, see NOTES section for ACTIVEUSERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphActiveUsersMetric[]
Parameter Sets: UpdateExpanded
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
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Authentications
Insights for authentications on apps registered in the tenant for a specified period.
To construct, see NOTES section for AUTHENTICATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationsMetric[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
monthlyUserInsightMetricsRoot
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphMonthlyUserInsightMetricsRoot
Parameter Sets: Update
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
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InactiveUsers

To construct, see NOTES section for INACTIVEUSERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMonthlyInactiveUsersMetric[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InactiveUsersByApplication

To construct, see NOTES section for INACTIVEUSERSBYAPPLICATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphMonthlyInactiveUsersByApplicationMetric[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MfaCompletions
Insights for MFA usage on apps registered in the tenant for a specified period.
To construct, see NOTES section for MFACOMPLETIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMfaCompletionMetric[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MfaRegisteredUsers

To construct, see NOTES section for MFAREGISTEREDUSERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMfaUserCountMetric[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Requests
Insights for all user requests on apps registered in the tenant for a specified period.
To construct, see NOTES section for REQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserRequestsMetric[]
Parameter Sets: UpdateExpanded
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

### -SignUps
Total sign-ups on apps registered in the tenant for a specified period.
To construct, see NOTES section for SIGNUPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserSignUpMetric[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Summary
Summary of all usage insights on apps registered in the tenant for a specified period.
To construct, see NOTES section for SUMMARY properties and create a hash table.

```yaml
Type: IMicrosoftGraphInsightSummary[]
Parameter Sets: UpdateExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMonthlyUserInsightMetricsRoot
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMonthlyUserInsightMetricsRoot
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ACTIVEUSERS `<IMicrosoftGraphActiveUsersMetric- `[]`>`: Insights for active users on apps registered in the tenant for a specified period.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AppId <String>]`: 
  - `[AppName <String>]`: 
  - `[Count <Int64?>]`: The total number of users who made at least one authentication request within the specified time period.
  - `[Country <String>]`: 
  - `[FactDate <DateTime?>]`: Date of the insight.
  - `[Language <String>]`: 
  - `[OS <String>]`: 

AUTHENTICATIONS `<IMicrosoftGraphAuthenticationsMetric- `[]`>`: Insights for authentications on apps registered in the tenant for a specified period.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Appid <String>]`: The ID of the Microsoft Entra application.
Supports $filter (eq).
  - `[AttemptsCount <Int64?>]`: The number of authentication requests made in the specified period.
Supports $filter (eq).
  - `[AuthFlow <String>]`: 
  - `[Browser <String>]`: 
  - `[Country <String>]`: The location where the customers authenticated from.
Supports $filter (eq).
  - `[FactDate <DateTime?>]`: The date of the user insight.
  - `[Failures <IMicrosoftGraphAuthenticationFailure- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Count <Int64?>]`: 
    - `[Reason <String>]`: 
    - `[ReasonCode <String>]`: authenticationFailureReasonCode
  - `[IdentityProvider <String>]`: 
  - `[Language <String>]`: 
  - `[OS <String>]`: The platform for the device that the customers used.
Supports $filter (eq).
  - `[SuccessCount <Int64?>]`: Number of successful authentication requests.
Supports $filter (eq).

BODYPARAMETER `<IMicrosoftGraphMonthlyUserInsightMetricsRoot>`: monthlyUserInsightMetricsRoot
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActiveUsers <IMicrosoftGraphActiveUsersMetric- `[]`>]`: Insights for active users on apps registered in the tenant for a specified period.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppId <String>]`: 
    - `[AppName <String>]`: 
    - `[Count <Int64?>]`: The total number of users who made at least one authentication request within the specified time period.
    - `[Country <String>]`: 
    - `[FactDate <DateTime?>]`: Date of the insight.
    - `[Language <String>]`: 
    - `[OS <String>]`: 
  - `[Authentications <IMicrosoftGraphAuthenticationsMetric- `[]`>]`: Insights for authentications on apps registered in the tenant for a specified period.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Appid <String>]`: The ID of the Microsoft Entra application.
Supports $filter (eq).
    - `[AttemptsCount <Int64?>]`: The number of authentication requests made in the specified period.
Supports $filter (eq).
    - `[AuthFlow <String>]`: 
    - `[Browser <String>]`: 
    - `[Country <String>]`: The location where the customers authenticated from.
Supports $filter (eq).
    - `[FactDate <DateTime?>]`: The date of the user insight.
    - `[Failures <IMicrosoftGraphAuthenticationFailure- `[]`>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Count <Int64?>]`: 
      - `[Reason <String>]`: 
      - `[ReasonCode <String>]`: authenticationFailureReasonCode
    - `[IdentityProvider <String>]`: 
    - `[Language <String>]`: 
    - `[OS <String>]`: The platform for the device that the customers used.
Supports $filter (eq).
    - `[SuccessCount <Int64?>]`: Number of successful authentication requests.
Supports $filter (eq).
  - `[InactiveUsers <IMicrosoftGraphMonthlyInactiveUsersMetric- `[]`>]`: 
    - `[AppId <String>]`: 
    - `[FactDate <DateTime?>]`: 
    - `[Inactive30DayCount <Int64?>]`: 
    - `[Inactive60DayCount <Int64?>]`: 
    - `[Inactive90DayCount <Int64?>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[InactiveCalendarMonthCount <Int64?>]`: 
  - `[InactiveUsersByApplication <IMicrosoftGraphMonthlyInactiveUsersByApplicationMetric- `[]`>]`: 
    - `[AppId <String>]`: 
    - `[FactDate <DateTime?>]`: 
    - `[Inactive30DayCount <Int64?>]`: 
    - `[Inactive60DayCount <Int64?>]`: 
    - `[Inactive90DayCount <Int64?>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[InactiveCalendarMonthCount <Int64?>]`: 
  - `[MfaCompletions <IMicrosoftGraphMfaCompletionMetric- `[]`>]`: Insights for MFA usage on apps registered in the tenant for a specified period.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppId <String>]`: The ID of the Microsoft Entra application.
Supports $filter (eq).
    - `[AttemptsCount <Int64?>]`: Number of users who attempted to sign up.
Supports $filter (eq).
    - `[Country <String>]`: 
    - `[FactDate <DateTime?>]`: The date of the user insight.
    - `[IdentityProvider <String>]`: 
    - `[Language <String>]`: 
    - `[MfaFailures <IMicrosoftGraphMfaFailure- `[]`>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Count <Int64?>]`: 
      - `[Reason <String>]`: 
      - `[ReasonCode <String>]`: mfaFailureReasonCode
    - `[MfaMethod <String>]`: The MFA authentication method used by the customers.
Supports $filter (eq).
    - `[OS <String>]`: The platform of the device that the customers used.
Supports $filter (eq).
    - `[SuccessCount <Int64?>]`: Number of users who signed up successfully.
Supports $filter (eq).
  - `[MfaRegisteredUsers <IMicrosoftGraphMfaUserCountMetric- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Count <Int64?>]`: 
    - `[FactDate <DateTime?>]`: 
    - `[MfaType <String>]`: mfaType
  - `[Requests <IMicrosoftGraphUserRequestsMetric- `[]`>]`: Insights for all user requests on apps registered in the tenant for a specified period.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppId <String>]`: 
    - `[Browser <String>]`: 
    - `[Country <String>]`: 
    - `[FactDate <DateTime?>]`: The date of the user insight.
    - `[IdentityProvider <String>]`: 
    - `[Language <String>]`: 
    - `[RequestCount <Int64?>]`: Number of requests to the tenant.
Supports $filter (eq).
  - `[SignUps <IMicrosoftGraphUserSignUpMetric- `[]`>]`: Total sign-ups on apps registered in the tenant for a specified period.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppId <String>]`: 
    - `[Browser <String>]`: 
    - `[Count <Int64?>]`: The total number of users who signed up in the specified period.
Supports $filter (eq).
    - `[Country <String>]`: 
    - `[FactDate <DateTime?>]`: The date of the user insight.
    - `[IdentityProvider <String>]`: 
    - `[Language <String>]`: 
    - `[OS <String>]`: The device plaform that the customers used.
Supports $filter (eq).
  - `[Summary <IMicrosoftGraphInsightSummary- `[]`>]`: Summary of all usage insights on apps registered in the tenant for a specified period.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ActiveUsers <Int64?>]`: Daily active users.
    - `[AppId <String>]`: The ID of the Microsoft Entra application.
    - `[AuthenticationCompletions <Int64?>]`: Daily authentication completions.
    - `[AuthenticationRequests <Int64?>]`: Daily authentication requests.
    - `[FactDate <DateTime?>]`: The date of the insight.
    - `[OS <String>]`: The platform for the device that the customers used.
Supports $filter (eq).
    - `[SecurityTextCompletions <Int64?>]`: Daily MFA SMS completions.
    - `[SecurityTextRequests <Int64?>]`: Daily MFA SMS requests.
    - `[SecurityVoiceCompletions <Int64?>]`: Daily MFA Voice completions.
    - `[SecurityVoiceRequests <Int64?>]`: Daily MFA Voice requests.

INACTIVEUSERS `<IMicrosoftGraphMonthlyInactiveUsersMetric- `[]`>`: .
  - `[AppId <String>]`: 
  - `[FactDate <DateTime?>]`: 
  - `[Inactive30DayCount <Int64?>]`: 
  - `[Inactive60DayCount <Int64?>]`: 
  - `[Inactive90DayCount <Int64?>]`: 
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[InactiveCalendarMonthCount <Int64?>]`: 

INACTIVEUSERSBYAPPLICATION `<IMicrosoftGraphMonthlyInactiveUsersByApplicationMetric- `[]`>`: .
  - `[AppId <String>]`: 
  - `[FactDate <DateTime?>]`: 
  - `[Inactive30DayCount <Int64?>]`: 
  - `[Inactive60DayCount <Int64?>]`: 
  - `[Inactive90DayCount <Int64?>]`: 
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[InactiveCalendarMonthCount <Int64?>]`: 

MFACOMPLETIONS `<IMicrosoftGraphMfaCompletionMetric- `[]`>`: Insights for MFA usage on apps registered in the tenant for a specified period.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AppId <String>]`: The ID of the Microsoft Entra application.
Supports $filter (eq).
  - `[AttemptsCount <Int64?>]`: Number of users who attempted to sign up.
Supports $filter (eq).
  - `[Country <String>]`: 
  - `[FactDate <DateTime?>]`: The date of the user insight.
  - `[IdentityProvider <String>]`: 
  - `[Language <String>]`: 
  - `[MfaFailures <IMicrosoftGraphMfaFailure- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Count <Int64?>]`: 
    - `[Reason <String>]`: 
    - `[ReasonCode <String>]`: mfaFailureReasonCode
  - `[MfaMethod <String>]`: The MFA authentication method used by the customers.
Supports $filter (eq).
  - `[OS <String>]`: The platform of the device that the customers used.
Supports $filter (eq).
  - `[SuccessCount <Int64?>]`: Number of users who signed up successfully.
Supports $filter (eq).

MFAREGISTEREDUSERS `<IMicrosoftGraphMfaUserCountMetric- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Count <Int64?>]`: 
  - `[FactDate <DateTime?>]`: 
  - `[MfaType <String>]`: mfaType

REQUESTS `<IMicrosoftGraphUserRequestsMetric- `[]`>`: Insights for all user requests on apps registered in the tenant for a specified period.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AppId <String>]`: 
  - `[Browser <String>]`: 
  - `[Country <String>]`: 
  - `[FactDate <DateTime?>]`: The date of the user insight.
  - `[IdentityProvider <String>]`: 
  - `[Language <String>]`: 
  - `[RequestCount <Int64?>]`: Number of requests to the tenant.
Supports $filter (eq).

SIGNUPS `<IMicrosoftGraphUserSignUpMetric- `[]`>`: Total sign-ups on apps registered in the tenant for a specified period.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AppId <String>]`: 
  - `[Browser <String>]`: 
  - `[Count <Int64?>]`: The total number of users who signed up in the specified period.
Supports $filter (eq).
  - `[Country <String>]`: 
  - `[FactDate <DateTime?>]`: The date of the user insight.
  - `[IdentityProvider <String>]`: 
  - `[Language <String>]`: 
  - `[OS <String>]`: The device plaform that the customers used.
Supports $filter (eq).

SUMMARY `<IMicrosoftGraphInsightSummary- `[]`>`: Summary of all usage insights on apps registered in the tenant for a specified period.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActiveUsers <Int64?>]`: Daily active users.
  - `[AppId <String>]`: The ID of the Microsoft Entra application.
  - `[AuthenticationCompletions <Int64?>]`: Daily authentication completions.
  - `[AuthenticationRequests <Int64?>]`: Daily authentication requests.
  - `[FactDate <DateTime?>]`: The date of the insight.
  - `[OS <String>]`: The platform for the device that the customers used.
Supports $filter (eq).
  - `[SecurityTextCompletions <Int64?>]`: Daily MFA SMS completions.
  - `[SecurityTextRequests <Int64?>]`: Daily MFA SMS requests.
  - `[SecurityVoiceCompletions <Int64?>]`: Daily MFA Voice completions.
  - `[SecurityVoiceRequests <Int64?>]`: Daily MFA Voice requests.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/update-mgbetareportuserinsightmonthly](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/update-mgbetareportuserinsightmonthly)
























