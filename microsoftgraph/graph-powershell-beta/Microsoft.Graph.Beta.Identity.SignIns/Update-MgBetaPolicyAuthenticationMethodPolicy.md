---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetapolicyauthenticationmethodpolicy
schema: 2.0.0
ms.subservice: entra-sign-in
---

# Update-MgBetaPolicyAuthenticationMethodPolicy

## SYNOPSIS
Update the properties of an authenticationMethodsPolicy object.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgPolicyAuthenticationMethodPolicy](/powershell/module/Microsoft.Graph.Identity.SignIns/Update-MgPolicyAuthenticationMethodPolicy?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaPolicyAuthenticationMethodPolicy [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>]
 [-AuthenticationMethodConfigurations <IMicrosoftGraphAuthenticationMethodConfiguration[]>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>] [-LastModifiedDateTime <DateTime>]
 [-MicrosoftAuthenticatorPlatformSettings <IMicrosoftGraphMicrosoftAuthenticatorPlatformSettings>]
 [-PolicyMigrationState <String>] [-PolicyVersion <String>] [-ReconfirmationInDays <Int32>]
 [-RegistrationEnforcement <IMicrosoftGraphRegistrationEnforcement>]
 [-ReportSuspiciousActivitySettings <IMicrosoftGraphReportSuspiciousActivitySettings>]
 [-SystemCredentialPreferences <IMicrosoftGraphSystemCredentialPreferences>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaPolicyAuthenticationMethodPolicy -BodyParameter <IMicrosoftGraphAuthenticationMethodsPolicy>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of an authenticationMethodsPolicy object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Policy.ReadWrite.AuthenticationMethod,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Policy.ReadWrite.AuthenticationMethod,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	registrationEnforcement = @{
		authenticationMethodsRegistrationCampaign = @{
			snoozeDurationInDays = 1
			enforceRegistrationAfterAllowedSnoozes = $true
			state = "enabled"
			excludeTargets = @(
			)
			includeTargets = @(
				@{
					id = "3ee3a9de-0a86-4e12-a287-9769accf1ba2"
					targetType = "group"
					targetedAuthenticationMethod = "microsoftAuthenticator"
				}
			)
		}
	}
	reportSuspiciousActivitySettings = @{
		state = "enabled"
		includeTarget = @{
			targetType = "group"
			id = "all_users"
		}
		voiceReportingCode = 0
	}
}

Update-MgBetaPolicyAuthenticationMethodPolicy -BodyParameter $params

```
This example shows how to use the Update-MgBetaPolicyAuthenticationMethodPolicy Cmdlet.


## PARAMETERS

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

### -AuthenticationMethodConfigurations
Represents the settings for each authentication method.
Automatically expanded on GET /policies/authenticationMethodsPolicy.
To construct, see NOTES section for AUTHENTICATIONMETHODCONFIGURATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationMethodConfiguration[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
authenticationMethodsPolicy
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationMethodsPolicy
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

### -Description
A description of the policy.

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

### -DisplayName
The name of the policy.

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

### -LastModifiedDateTime
The date and time of the last update to the policy.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MicrosoftAuthenticatorPlatformSettings
microsoftAuthenticatorPlatformSettings
To construct, see NOTES section for MICROSOFTAUTHENTICATORPLATFORMSETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMicrosoftAuthenticatorPlatformSettings
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PolicyMigrationState
authenticationMethodsPolicyMigrationState

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

### -PolicyVersion
The version of the policy in use.

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

### -ReconfirmationInDays
Days before the user will be asked to reconfirm their method.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -RegistrationEnforcement
registrationEnforcement
To construct, see NOTES section for REGISTRATIONENFORCEMENT properties and create a hash table.

```yaml
Type: IMicrosoftGraphRegistrationEnforcement
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReportSuspiciousActivitySettings
reportSuspiciousActivitySettings
To construct, see NOTES section for REPORTSUSPICIOUSACTIVITYSETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphReportSuspiciousActivitySettings
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

### -SystemCredentialPreferences
systemCredentialPreferences
To construct, see NOTES section for SYSTEMCREDENTIALPREFERENCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSystemCredentialPreferences
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAuthenticationMethodsPolicy
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAuthenticationMethodsPolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

AUTHENTICATIONMETHODCONFIGURATIONS `<IMicrosoftGraphAuthenticationMethodConfiguration- `[]`>`: Represents the settings for each authentication method.
Automatically expanded on GET /policies/authenticationMethodsPolicy.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ExcludeTargets <IMicrosoftGraphExcludeTarget- `[]`>]`: Groups of users that are excluded from a policy.
    - `[Id <String>]`: The object identifier of a Microsoft Entra group.
    - `[TargetType <String>]`: authenticationMethodTargetType
  - `[State <String>]`: authenticationMethodState

BODYPARAMETER `<IMicrosoftGraphAuthenticationMethodsPolicy>`: authenticationMethodsPolicy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AuthenticationMethodConfigurations <IMicrosoftGraphAuthenticationMethodConfiguration- `[]`>]`: Represents the settings for each authentication method.
Automatically expanded on GET /policies/authenticationMethodsPolicy.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ExcludeTargets <IMicrosoftGraphExcludeTarget- `[]`>]`: Groups of users that are excluded from a policy.
      - `[Id <String>]`: The object identifier of a Microsoft Entra group.
      - `[TargetType <String>]`: authenticationMethodTargetType
    - `[State <String>]`: authenticationMethodState
  - `[Description <String>]`: A description of the policy.
  - `[DisplayName <String>]`: The name of the policy.
  - `[LastModifiedDateTime <DateTime?>]`: The date and time of the last update to the policy.
  - `[MicrosoftAuthenticatorPlatformSettings <IMicrosoftGraphMicrosoftAuthenticatorPlatformSettings>]`: microsoftAuthenticatorPlatformSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[EnforceAppPin <IMicrosoftGraphEnforceAppPin>]`: enforceAppPIN
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ExcludeTargets <IMicrosoftGraphExcludeTarget- `[]`>]`: 
      - `[IncludeTargets <IMicrosoftGraphIncludeTarget- `[]`>]`: 
        - `[Id <String>]`: The ID of the entity targeted.
        - `[TargetType <String>]`: authenticationMethodTargetType
  - `[PolicyMigrationState <String>]`: authenticationMethodsPolicyMigrationState
  - `[PolicyVersion <String>]`: The version of the policy in use.
  - `[ReconfirmationInDays <Int32?>]`: Days before the user will be asked to reconfirm their method.
  - `[RegistrationEnforcement <IMicrosoftGraphRegistrationEnforcement>]`: registrationEnforcement
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AuthenticationMethodsRegistrationCampaign <IMicrosoftGraphAuthenticationMethodsRegistrationCampaign>]`: authenticationMethodsRegistrationCampaign
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[EnforceRegistrationAfterAllowedSnoozes <Boolean?>]`: Specifies whether a user is required to perform registration after snoozing 3 times.
If true, the user is required to register after 3 snoozes.
If false, the user can snooze indefinitely.
The default value is true.
      - `[ExcludeTargets <IMicrosoftGraphExcludeTarget- `[]`>]`: Users and groups of users that are excluded from being prompted to set up the authentication method.
      - `[IncludeTargets <IMicrosoftGraphAuthenticationMethodsRegistrationCampaignIncludeTarget- `[]`>]`: Users and groups of users that are prompted to set up the authentication method.
        - `[Id <String>]`: The object identifier of a Microsoft Entra user or group.
        - `[TargetType <String>]`: authenticationMethodTargetType
        - `[TargetedAuthenticationMethod <String>]`: The authentication method that the user is prompted to register.
The value must be microsoftAuthenticator.
      - `[SnoozeDurationInDays <Int32?>]`: Specifies the number of days that the user sees a prompt again if they select 'Not now' and snoozes the prompt.
Minimum 0 days.
Maximum: 14 days.
If the value is 0 - The user is prompted during every MFA attempt.
      - `[State <String>]`: advancedConfigState
  - `[ReportSuspiciousActivitySettings <IMicrosoftGraphReportSuspiciousActivitySettings>]`: reportSuspiciousActivitySettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IncludeTarget <IMicrosoftGraphIncludeTarget>]`: includeTarget
    - `[State <String>]`: advancedConfigState
    - `[VoiceReportingCode <Int32?>]`: Specifies the number the user enters on their phone to report the MFA prompt as suspicious.
  - `[SystemCredentialPreferences <IMicrosoftGraphSystemCredentialPreferences>]`: systemCredentialPreferences
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ExcludeTargets <IMicrosoftGraphExcludeTarget- `[]`>]`: Users and groups excluded from the preferred authentication method experience of the system.
    - `[IncludeTargets <IMicrosoftGraphIncludeTarget- `[]`>]`: Users and groups included in the preferred authentication method experience of the system.
    - `[State <String>]`: advancedConfigState

MICROSOFTAUTHENTICATORPLATFORMSETTINGS `<IMicrosoftGraphMicrosoftAuthenticatorPlatformSettings>`: microsoftAuthenticatorPlatformSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[EnforceAppPin <IMicrosoftGraphEnforceAppPin>]`: enforceAppPIN
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ExcludeTargets <IMicrosoftGraphExcludeTarget- `[]`>]`: 
      - `[Id <String>]`: The object identifier of a Microsoft Entra group.
      - `[TargetType <String>]`: authenticationMethodTargetType
    - `[IncludeTargets <IMicrosoftGraphIncludeTarget- `[]`>]`: 
      - `[Id <String>]`: The ID of the entity targeted.
      - `[TargetType <String>]`: authenticationMethodTargetType

REGISTRATIONENFORCEMENT `<IMicrosoftGraphRegistrationEnforcement>`: registrationEnforcement
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AuthenticationMethodsRegistrationCampaign <IMicrosoftGraphAuthenticationMethodsRegistrationCampaign>]`: authenticationMethodsRegistrationCampaign
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[EnforceRegistrationAfterAllowedSnoozes <Boolean?>]`: Specifies whether a user is required to perform registration after snoozing 3 times.
If true, the user is required to register after 3 snoozes.
If false, the user can snooze indefinitely.
The default value is true.
    - `[ExcludeTargets <IMicrosoftGraphExcludeTarget- `[]`>]`: Users and groups of users that are excluded from being prompted to set up the authentication method.
      - `[Id <String>]`: The object identifier of a Microsoft Entra group.
      - `[TargetType <String>]`: authenticationMethodTargetType
    - `[IncludeTargets <IMicrosoftGraphAuthenticationMethodsRegistrationCampaignIncludeTarget- `[]`>]`: Users and groups of users that are prompted to set up the authentication method.
      - `[Id <String>]`: The object identifier of a Microsoft Entra user or group.
      - `[TargetType <String>]`: authenticationMethodTargetType
      - `[TargetedAuthenticationMethod <String>]`: The authentication method that the user is prompted to register.
The value must be microsoftAuthenticator.
    - `[SnoozeDurationInDays <Int32?>]`: Specifies the number of days that the user sees a prompt again if they select 'Not now' and snoozes the prompt.
Minimum 0 days.
Maximum: 14 days.
If the value is 0 - The user is prompted during every MFA attempt.
    - `[State <String>]`: advancedConfigState

REPORTSUSPICIOUSACTIVITYSETTINGS `<IMicrosoftGraphReportSuspiciousActivitySettings>`: reportSuspiciousActivitySettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IncludeTarget <IMicrosoftGraphIncludeTarget>]`: includeTarget
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The ID of the entity targeted.
    - `[TargetType <String>]`: authenticationMethodTargetType
  - `[State <String>]`: advancedConfigState
  - `[VoiceReportingCode <Int32?>]`: Specifies the number the user enters on their phone to report the MFA prompt as suspicious.

SYSTEMCREDENTIALPREFERENCES `<IMicrosoftGraphSystemCredentialPreferences>`: systemCredentialPreferences
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ExcludeTargets <IMicrosoftGraphExcludeTarget- `[]`>]`: Users and groups excluded from the preferred authentication method experience of the system.
    - `[Id <String>]`: The object identifier of a Microsoft Entra group.
    - `[TargetType <String>]`: authenticationMethodTargetType
  - `[IncludeTargets <IMicrosoftGraphIncludeTarget- `[]`>]`: Users and groups included in the preferred authentication method experience of the system.
    - `[Id <String>]`: The ID of the entity targeted.
    - `[TargetType <String>]`: authenticationMethodTargetType
  - `[State <String>]`: advancedConfigState

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetapolicyauthenticationmethodpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetapolicyauthenticationmethodpolicy)

[https://learn.microsoft.com/graph/api/authenticationmethodspolicy-update?view=graph-rest-beta](https://learn.microsoft.com/graph/api/authenticationmethodspolicy-update?view=graph-rest-beta)























