---
external help file: Microsoft.Graph.Users.Actions-help.xml
Module Name: Microsoft.Graph.Users.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/revoke-mgusersigninsession
schema: 2.0.0
ms.subservice: entra-users
---

# Revoke-MgUserSignInSession

## SYNOPSIS
Invalidates all the refresh tokens issued to applications for a user (and session cookies in a user's browser), by resetting the signInSessionsValidFromDateTime user property to the current date-time.
Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.
This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they consented to previously, independent of device.

> [!NOTE]
> To view the beta release of this cmdlet, view [Revoke-MgBetaUserSignInSession](/powershell/module/Microsoft.Graph.Beta.Users.Actions/Revoke-MgBetaUserSignInSession?view=graph-powershell-beta)

## SYNTAX

### Revoke (Default)
```
Revoke-MgUserSignInSession -UserId <String> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RevokeViaIdentity
```
Revoke-MgUserSignInSession -InputObject <IUsersActionsIdentity> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invalidates all the refresh tokens issued to applications for a user (and session cookies in a user's browser), by resetting the signInSessionsValidFromDateTime user property to the current date-time.
Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.
This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they consented to previously, independent of device.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | User.RevokeSessions.All, User.ReadWrite.All, Directory.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | User.RevokeSessions.All, User.ReadWrite.All, Directory.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
Revoke-MgUserSignInSession -UserId $userId

```
This example shows how to use the Revoke-MgUserSignInSession Cmdlet.


## PARAMETERS

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IUsersActionsIdentity
Parameter Sets: RevokeViaIdentity
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

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: Revoke
Aliases:

Required: True
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

### Microsoft.Graph.PowerShell.Models.IUsersActionsIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IUsersActionsIdentity>`: Identity Parameter
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/revoke-mgusersigninsession](https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/revoke-mgusersigninsession)

[https://learn.microsoft.com/graph/api/user-revokesigninsessions?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/user-revokesigninsessions?view=graph-rest-1.0)























