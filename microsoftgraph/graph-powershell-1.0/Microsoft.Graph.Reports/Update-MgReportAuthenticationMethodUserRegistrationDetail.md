---
external help file: Microsoft.Graph.Reports-help.xml
Module Name: Microsoft.Graph.Reports
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.reports/update-mgreportauthenticationmethoduserregistrationdetail
schema: 2.0.0
---

# Update-MgReportAuthenticationMethodUserRegistrationDetail

## SYNOPSIS
Update the navigation property userRegistrationDetails in reports

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaReportAuthenticationMethodUserRegistrationDetail](/powershell/module/Microsoft.Graph.Beta.Reports/Update-MgBetaReportAuthenticationMethodUserRegistrationDetail?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgReportAuthenticationMethodUserRegistrationDetail -UserRegistrationDetailsId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Id <String>] [-IsAdmin]
 [-IsMfaCapable] [-IsMfaRegistered] [-IsPasswordlessCapable] [-IsSsprCapable] [-IsSsprEnabled]
 [-IsSsprRegistered] [-IsSystemPreferredAuthenticationMethodEnabled] [-LastUpdatedDateTime <DateTime>]
 [-MethodsRegistered <String[]>] [-SystemPreferredAuthenticationMethods <String[]>] [-UserDisplayName <String>]
 [-UserPreferredMethodForSecondaryAuthentication <String>] [-UserPrincipalName <String>] [-UserType <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgReportAuthenticationMethodUserRegistrationDetail -UserRegistrationDetailsId <String>
 -BodyParameter <IMicrosoftGraphUserRegistrationDetails> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgReportAuthenticationMethodUserRegistrationDetail -InputObject <IReportsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Id <String>] [-IsAdmin]
 [-IsMfaCapable] [-IsMfaRegistered] [-IsPasswordlessCapable] [-IsSsprCapable] [-IsSsprEnabled]
 [-IsSsprRegistered] [-IsSystemPreferredAuthenticationMethodEnabled] [-LastUpdatedDateTime <DateTime>]
 [-MethodsRegistered <String[]>] [-SystemPreferredAuthenticationMethods <String[]>] [-UserDisplayName <String>]
 [-UserPreferredMethodForSecondaryAuthentication <String>] [-UserPrincipalName <String>] [-UserType <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgReportAuthenticationMethodUserRegistrationDetail -InputObject <IReportsIdentity>
 -BodyParameter <IMicrosoftGraphUserRegistrationDetails> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property userRegistrationDetails in reports

## EXAMPLES

## PARAMETERS

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

### -BodyParameter
userRegistrationDetails
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserRegistrationDetails
Parameter Sets: Update, UpdateViaIdentity
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
Type: IReportsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsAdmin
Indicates whether the user has an admin role in the tenant.
This value can be used to check the authentication methods that privileged accounts are registered for and capable of.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsMfaCapable
Indicates whether the user has registered a strong authentication method for multifactor authentication.
The method must be allowed by the authentication methods policy.
Supports $filter (eq).

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsMfaRegistered
Indicates whether the user has registered a strong authentication method for multifactor authentication.
The method may not necessarily be allowed by the authentication methods policy.
Supports $filter (eq).

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsPasswordlessCapable
Indicates whether the user has registered a passwordless strong authentication method (including FIDO2, Windows Hello for Business, and Microsoft Authenticator (Passwordless)) that is allowed by the authentication methods policy.
Supports $filter (eq).

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsSsprCapable
Indicates whether the user has registered the required number of authentication methods for self-service password reset and the user is allowed to perform self-service password reset by policy.
Supports $filter (eq).

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsSsprEnabled
Indicates whether the user is allowed to perform self-service password reset by policy.
The user may not necessarily have registered the required number of authentication methods for self-service password reset.
Supports $filter (eq).

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsSsprRegistered
Indicates whether the user has registered the required number of authentication methods for self-service password reset.
The user may not necessarily be allowed to perform self-service password reset by policy.
Supports $filter (eq).

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsSystemPreferredAuthenticationMethodEnabled
Indicates whether system preferred authentication method is enabled.
If enabled, the system dynamically determines the most secure authentication method among the methods registered by the user.
Supports $filter (eq).

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastUpdatedDateTime
The date and time (UTC) when the report was last updated.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
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

### -MethodsRegistered
Collection of authentication methods registered, such as mobilePhone, email, passKeyDeviceBound.
Supports $filter (any with eq).

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

### -SystemPreferredAuthenticationMethods
Collection of authentication methods that the system determined to be the most secure authentication methods among the registered methods for second factor authentication.
Possible values are: push, oath, voiceMobile, voiceAlternateMobile, voiceOffice, sms, none, unknownFutureValue.
Supports $filter (any with eq).

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

### -UserDisplayName
The user display name, such as Adele Vance.
Supports $filter (eq, startsWith) and $orderby.

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

### -UserPreferredMethodForSecondaryAuthentication
userDefaultAuthenticationMethod

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

### -UserPrincipalName
The user principal name, such as AdeleV@contoso.com.
Supports $filter (eq, startsWith) and $orderby.

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

### -UserRegistrationDetailsId
The unique identifier of userRegistrationDetails

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

### -UserType
signInUserType

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUserRegistrationDetails
### Microsoft.Graph.PowerShell.Models.IReportsIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUserRegistrationDetails
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphUserRegistrationDetails>`: userRegistrationDetails
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[IsAdmin <Boolean?>]`: Indicates whether the user has an admin role in the tenant.
This value can be used to check the authentication methods that privileged accounts are registered for and capable of.
  - `[IsMfaCapable <Boolean?>]`: Indicates whether the user has registered a strong authentication method for multifactor authentication.
The method must be allowed by the authentication methods policy.
Supports $filter (eq).
  - `[IsMfaRegistered <Boolean?>]`: Indicates whether the user has registered a strong authentication method for multifactor authentication.
The method may not necessarily be allowed by the authentication methods policy.
Supports $filter (eq).
  - `[IsPasswordlessCapable <Boolean?>]`: Indicates whether the user has registered a passwordless strong authentication method (including FIDO2, Windows Hello for Business, and Microsoft Authenticator (Passwordless)) that is allowed by the authentication methods policy.
Supports $filter (eq).
  - `[IsSsprCapable <Boolean?>]`: Indicates whether the user has registered the required number of authentication methods for self-service password reset and the user is allowed to perform self-service password reset by policy.
Supports $filter (eq).
  - `[IsSsprEnabled <Boolean?>]`: Indicates whether the user is allowed to perform self-service password reset by policy.
The user may not necessarily have registered the required number of authentication methods for self-service password reset.
Supports $filter (eq).
  - `[IsSsprRegistered <Boolean?>]`: Indicates whether the user has registered the required number of authentication methods for self-service password reset.
The user may not necessarily be allowed to perform self-service password reset by policy.
Supports $filter (eq).
  - `[IsSystemPreferredAuthenticationMethodEnabled <Boolean?>]`: Indicates whether system preferred authentication method is enabled.
If enabled, the system dynamically determines the most secure authentication method among the methods registered by the user.
Supports $filter (eq).
  - `[LastUpdatedDateTime <DateTime?>]`: The date and time (UTC) when the report was last updated.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[MethodsRegistered <String- `[]`>]`: Collection of authentication methods registered, such as mobilePhone, email, passKeyDeviceBound.
Supports $filter (any with eq).
  - `[SystemPreferredAuthenticationMethods <String- `[]`>]`: Collection of authentication methods that the system determined to be the most secure authentication methods among the registered methods for second factor authentication.
Possible values are: push, oath, voiceMobile, voiceAlternateMobile, voiceOffice, sms, none, unknownFutureValue.
Supports $filter (any with eq).
  - `[UserDisplayName <String>]`: The user display name, such as Adele Vance.
Supports $filter (eq, startsWith) and $orderby.
  - `[UserPreferredMethodForSecondaryAuthentication <String>]`: userDefaultAuthenticationMethod
  - `[UserPrincipalName <String>]`: The user principal name, such as AdeleV@contoso.com.
Supports $filter (eq, startsWith) and $orderby.
  - `[UserType <String>]`: signInUserType

INPUTOBJECT `<IReportsIdentity>`: Identity Parameter
  - `[Date <DateTime?>]`: Usage: date={date}
  - `[DeviceManagementExportJobId <String>]`: The unique identifier of deviceManagementExportJob
  - `[DirectoryAuditId <String>]`: The unique identifier of directoryAudit
  - `[EndDateTime <DateTime?>]`: Usage: endDateTime={endDateTime}
  - `[Filter <String>]`: Usage: filter='{filter}'
  - `[GroupId <String>]`: Usage: groupId='{groupId}'
  - `[IncludedUserRoles <String>]`: Usage: includedUserRoles='{includedUserRoles}'
  - `[IncludedUserTypes <String>]`: Usage: includedUserTypes='{includedUserTypes}'
  - `[ManifestId <String>]`: The unique identifier of manifest
  - `[OperationId <String>]`: The unique identifier of operation
  - `[Period <String>]`: Usage: period='{period}'
  - `[PrintUsageByPrinterId <String>]`: The unique identifier of printUsageByPrinter
  - `[PrintUsageByUserId <String>]`: The unique identifier of printUsageByUser
  - `[PrinterId <String>]`: Usage: printerId='{printerId}'
  - `[ProvisioningObjectSummaryId <String>]`: The unique identifier of provisioningObjectSummary
  - `[SignInId <String>]`: The unique identifier of signIn
  - `[Skip <Int32?>]`: Usage: skip={skip}
  - `[SkipToken <String>]`: Usage: skipToken='{skipToken}'
  - `[StartDateTime <DateTime?>]`: Usage: startDateTime={startDateTime}
  - `[Top <Int32?>]`: Usage: top={top}
  - `[UserId <String>]`: Usage: userId='{userId}'
  - `[UserRegistrationDetailsId <String>]`: The unique identifier of userRegistrationDetails

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.reports/update-mgreportauthenticationmethoduserregistrationdetail](https://learn.microsoft.com/powershell/module/microsoft.graph.reports/update-mgreportauthenticationmethoduserregistrationdetail)
























