---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgpolicyauthorizationpolicy
schema: 2.0.0
ms.subservice: entra-sign-in
---

# Update-MgPolicyAuthorizationPolicy

## SYNOPSIS
Update the properties of an authorizationPolicy object.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaPolicyAuthorizationPolicy](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/Update-MgBetaPolicyAuthorizationPolicy?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgPolicyAuthorizationPolicy [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AllowEmailVerifiedUsersToJoinOrganization] [-AllowInvitesFrom <String>] [-AllowUserConsentForRiskyApps]
 [-AllowedToSignUpEmailBasedSubscriptions] [-AllowedToUseSspr] [-BlockMsolPowerShell]
 [-DefaultUserRolePermissions <IMicrosoftGraphDefaultUserRolePermissions>] [-DeletedDateTime <DateTime>]
 [-Description <String>] [-DisplayName <String>] [-GuestUserRoleId <String>] [-Id <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgPolicyAuthorizationPolicy -BodyParameter <IMicrosoftGraphAuthorizationPolicy>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of an authorizationPolicy object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Policy.ReadWrite.Authorization,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Policy.ReadWrite.Authorization,  |

## EXAMPLES
### Example 1: Update or set Guest user access level for the tenant

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	allowEmailVerifiedUsersToJoinOrganization = $false
}

Update-MgPolicyAuthorizationPolicy -BodyParameter $params

```
This example will update or set guest user access level for the tenant

### Example 2: Block MSOL PowerShell in tenant

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	blockMsolPowerShell = $true
}

Update-MgPolicyAuthorizationPolicy -BodyParameter $params

```
This example will block msol powershell in tenant

### Example 3: Disable default user role's permission to create applications

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	defaultUserRolePermissions = @{
		allowedToCreateApps = $false
	}
}

Update-MgPolicyAuthorizationPolicy -BodyParameter $params

```
This example will disable default user role's permission to create applications

### Example 4: Enable default user role to use Self-Serve Password Reset feature

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	allowedToUseSSPR = $true
}

Update-MgPolicyAuthorizationPolicy -BodyParameter $params

```
This example will enable default user role to use self-serve password reset feature

### Example 5: Disable user consent to apps for default user role

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	defaultUserRolePermissions = @{
		permissionGrantPoliciesAssigned = @(
		)
	}
}

Update-MgPolicyAuthorizationPolicy -BodyParameter $params

```
This example will disable user consent to apps for default user role

### Example 6: Enable user consent to apps, subject to app consent policy

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	defaultUserRolePermissions = @{
		permissionGrantPoliciesAssigned = @(
		"managePermissionGrantsForSelf.microsoft-user-default-low"
	)
}
}

Update-MgPolicyAuthorizationPolicy -BodyParameter $params

```
This example will enable user consent to apps, subject to app consent policy


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

### -AllowedToSignUpEmailBasedSubscriptions
Indicates whether users can sign up for email based subscriptions.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowedToUseSspr
Indicates whether administrators of the tenant can use the Self-Service Password Reset (SSPR).
For more information, see Self-service password reset for administrators.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowEmailVerifiedUsersToJoinOrganization
Indicates whether a user can join the tenant by email validation.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowInvitesFrom
allowInvitesFrom

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

### -AllowUserConsentForRiskyApps
Indicates whether user consent for risky apps is allowed.
We recommend keeping allowUserConsentForRiskyApps as false.
Default value is false.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BlockMsolPowerShell
To disable the use of MSOL PowerShell, set this property to true.
This also disables user-based access to the legacy service endpoint used by MSOL PowerShell.
This doesn't affect Microsoft Entra Connect or Microsoft Graph.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
authorizationPolicy
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthorizationPolicy
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

### -DefaultUserRolePermissions
defaultUserRolePermissions
To construct, see NOTES section for DEFAULTUSERROLEPERMISSIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDefaultUserRolePermissions
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeletedDateTime
Date and time when this object was deleted.
Always null when the object hasn't been deleted.

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

### -Description
Description for this policy.
Required.

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
Display name for this policy.
Required.

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

### -GuestUserRoleId
Represents role templateId for the role that should be granted to guests.
Currently following roles are supported: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuthorizationPolicy
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuthorizationPolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphAuthorizationPolicy>`: authorizationPolicy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Description <String>]`: Description for this policy.
Required.
  - `[DisplayName <String>]`: Display name for this policy.
Required.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AllowEmailVerifiedUsersToJoinOrganization <Boolean?>]`: Indicates whether a user can join the tenant by email validation.
  - `[AllowInvitesFrom <String>]`: allowInvitesFrom
  - `[AllowUserConsentForRiskyApps <Boolean?>]`: Indicates whether user consent for risky apps is allowed.
We recommend keeping allowUserConsentForRiskyApps as false.
Default value is false.
  - `[AllowedToSignUpEmailBasedSubscriptions <Boolean?>]`: Indicates whether users can sign up for email based subscriptions.
  - `[AllowedToUseSspr <Boolean?>]`: Indicates whether administrators of the tenant can use the Self-Service Password Reset (SSPR).
For more information, see Self-service password reset for administrators.
  - `[BlockMsolPowerShell <Boolean?>]`: To disable the use of MSOL PowerShell, set this property to true.
This also disables user-based access to the legacy service endpoint used by MSOL PowerShell.
This doesn't affect Microsoft Entra Connect or Microsoft Graph.
  - `[DefaultUserRolePermissions <IMicrosoftGraphDefaultUserRolePermissions>]`: defaultUserRolePermissions
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowedToCreateApps <Boolean?>]`: Indicates whether the default user role can create applications.
This setting corresponds to the Users can register applications setting in the User settings menu in the Microsoft Entra admin center.
    - `[AllowedToCreateSecurityGroups <Boolean?>]`: Indicates whether the default user role can create security groups.
This setting corresponds to the following menus in the Microsoft Entra admin center:  The Users can create security groups in Microsoft Entra admin centers, API or PowerShell setting in the Group settings menu.
Users can create security groups setting in the User settings menu.
    - `[AllowedToCreateTenants <Boolean?>]`: Indicates whether the default user role can create tenants.
This setting corresponds to the Restrict non-admin users from creating tenants setting in the User settings menu in the Microsoft Entra admin center.
When this setting is false, users assigned the Tenant Creator role can still create tenants.
    - `[AllowedToReadBitlockerKeysForOwnedDevice <Boolean?>]`: Indicates whether the registered owners of a device can read their own BitLocker recovery keys with default user role.
    - `[AllowedToReadOtherUsers <Boolean?>]`: Indicates whether the default user role can read other users.
DO NOT SET THIS VALUE TO false.
    - `[PermissionGrantPoliciesAssigned <String- `[]`>]`: Indicates if user consent to apps is allowed, and if it is, which permission to grant consent and which app consent policy (permissionGrantPolicy) govern the permission for users to grant consent.
Value should be in the format managePermissionGrantsForSelf.{id}, where {id} is the id of a built-in or custom app consent policy.
An empty list indicates user consent to apps is disabled.
  - `[GuestUserRoleId <String>]`: Represents role templateId for the role that should be granted to guests.
Currently following roles are supported:  User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).

DEFAULTUSERROLEPERMISSIONS `<IMicrosoftGraphDefaultUserRolePermissions>`: defaultUserRolePermissions
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AllowedToCreateApps <Boolean?>]`: Indicates whether the default user role can create applications.
This setting corresponds to the Users can register applications setting in the User settings menu in the Microsoft Entra admin center.
  - `[AllowedToCreateSecurityGroups <Boolean?>]`: Indicates whether the default user role can create security groups.
This setting corresponds to the following menus in the Microsoft Entra admin center:  The Users can create security groups in Microsoft Entra admin centers, API or PowerShell setting in the Group settings menu.
Users can create security groups setting in the User settings menu.
  - `[AllowedToCreateTenants <Boolean?>]`: Indicates whether the default user role can create tenants.
This setting corresponds to the Restrict non-admin users from creating tenants setting in the User settings menu in the Microsoft Entra admin center.
When this setting is false, users assigned the Tenant Creator role can still create tenants.
  - `[AllowedToReadBitlockerKeysForOwnedDevice <Boolean?>]`: Indicates whether the registered owners of a device can read their own BitLocker recovery keys with default user role.
  - `[AllowedToReadOtherUsers <Boolean?>]`: Indicates whether the default user role can read other users.
DO NOT SET THIS VALUE TO false.
  - `[PermissionGrantPoliciesAssigned <String- `[]`>]`: Indicates if user consent to apps is allowed, and if it is, which permission to grant consent and which app consent policy (permissionGrantPolicy) govern the permission for users to grant consent.
Value should be in the format managePermissionGrantsForSelf.{id}, where {id} is the id of a built-in or custom app consent policy.
An empty list indicates user consent to apps is disabled.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgpolicyauthorizationpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgpolicyauthorizationpolicy)

[https://learn.microsoft.com/graph/api/authorizationpolicy-update?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/authorizationpolicy-update?view=graph-rest-1.0)























