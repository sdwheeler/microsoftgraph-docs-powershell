---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaidentityconditionalaccessauthenticationstrength
schema: 2.0.0
---

# Update-MgBetaIdentityConditionalAccessAuthenticationStrength

## SYNOPSIS
Update the navigation property authenticationStrengths in identity

## SYNTAX

### UpdateExpanded1 (Default)
```
Update-MgBetaIdentityConditionalAccessAuthenticationStrength [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AuthenticationCombinations <String[]>]
 [-AuthenticationMethodModes <IMicrosoftGraphAuthenticationMethodModeDetail[]>] [-Combinations <String[]>]
 [-Id <String>] [-Policies <IMicrosoftGraphAuthenticationStrengthPolicy[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update1
```
Update-MgBetaIdentityConditionalAccessAuthenticationStrength
 -BodyParameter <IMicrosoftGraphAuthenticationStrengthRoot> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property authenticationStrengths in identity

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AuthenticationCombinations
A collection of all valid authentication method combinations in the system.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AuthenticationMethodModes
Names and descriptions of all valid authentication method modes in the system.
To construct, see NOTES section for AUTHENTICATIONMETHODMODES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationMethodModeDetail[]
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
authenticationStrengthRoot
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationStrengthRoot
Parameter Sets: Update1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Combinations


```yaml
Type: String[]
Parameter Sets: UpdateExpanded1
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
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Policies
A collection of authentication strength policies that exist for this tenant, including both built-in and custom policies.
To construct, see NOTES section for POLICIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationStrengthPolicy[]
Parameter Sets: UpdateExpanded1
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAuthenticationStrengthRoot
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAuthenticationStrengthRoot
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

AUTHENTICATIONMETHODMODES `<IMicrosoftGraphAuthenticationMethodModeDetail- `[]`>`: Names and descriptions of all valid authentication method modes in the system.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AuthenticationMethod <String>]`: baseAuthenticationMethod
  - `[DisplayName <String>]`: The display name of this mode

BODYPARAMETER `<IMicrosoftGraphAuthenticationStrengthRoot>`: authenticationStrengthRoot
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AuthenticationCombinations <String- `[]`>]`: A collection of all valid authentication method combinations in the system.
  - `[AuthenticationMethodModes <IMicrosoftGraphAuthenticationMethodModeDetail- `[]`>]`: Names and descriptions of all valid authentication method modes in the system.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AuthenticationMethod <String>]`: baseAuthenticationMethod
    - `[DisplayName <String>]`: The display name of this mode
  - `[Combinations <String- `[]`>]`: 
  - `[Policies <IMicrosoftGraphAuthenticationStrengthPolicy- `[]`>]`: A collection of authentication strength policies that exist for this tenant, including both built-in and custom policies.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AllowedCombinations <String- `[]`>]`: A collection of authentication method modes that are required be used to satify this authentication strength.
    - `[CombinationConfigurations <IMicrosoftGraphAuthenticationCombinationConfiguration- `[]`>]`: Settings that may be used to require specific types or instances of an authentication method to be used when authenticating with a specified combination of authentication methods.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AppliesToCombinations <String- `[]`>]`: Which authentication method combinations this configuration applies to.
Must be an allowedCombinations object defined for the authenticationStrengthPolicy.
For fido2combinationConfigurations use 'fido2', for x509certificatecombinationconfiguration use 'x509CertificateSingleFactor' or 'x509CertificateMultiFactor'.
    - `[CreatedDateTime <DateTime?>]`: The datetime when this policy was created.
    - `[Description <String>]`: The human-readable description of this policy.
    - `[DisplayName <String>]`: The human-readable display name of this policy.
Supports $filter (eq, ne, not , and in).
    - `[ModifiedDateTime <DateTime?>]`: The datetime when this policy was last modified.
    - `[PolicyType <String>]`: authenticationStrengthPolicyType
    - `[RequirementsSatisfied <String>]`: authenticationStrengthRequirements

POLICIES `<IMicrosoftGraphAuthenticationStrengthPolicy- `[]`>`: A collection of authentication strength policies that exist for this tenant, including both built-in and custom policies.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AllowedCombinations <String- `[]`>]`: A collection of authentication method modes that are required be used to satify this authentication strength.
  - `[CombinationConfigurations <IMicrosoftGraphAuthenticationCombinationConfiguration- `[]`>]`: Settings that may be used to require specific types or instances of an authentication method to be used when authenticating with a specified combination of authentication methods.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppliesToCombinations <String- `[]`>]`: Which authentication method combinations this configuration applies to.
Must be an allowedCombinations object defined for the authenticationStrengthPolicy.
For fido2combinationConfigurations use 'fido2', for x509certificatecombinationconfiguration use 'x509CertificateSingleFactor' or 'x509CertificateMultiFactor'.
  - `[CreatedDateTime <DateTime?>]`: The datetime when this policy was created.
  - `[Description <String>]`: The human-readable description of this policy.
  - `[DisplayName <String>]`: The human-readable display name of this policy.
Supports $filter (eq, ne, not , and in).
  - `[ModifiedDateTime <DateTime?>]`: The datetime when this policy was last modified.
  - `[PolicyType <String>]`: authenticationStrengthPolicyType
  - `[RequirementsSatisfied <String>]`: authenticationStrengthRequirements

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaidentityconditionalaccessauthenticationstrength](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/update-mgbetaidentityconditionalaccessauthenticationstrength)
























