---
external help file: Microsoft.Graph.Users.Actions-help.xml
Module Name: Microsoft.Graph.Users.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/invoke-mglicenseuser
schema: 2.0.0
ms.subservice: entra-users
---

# Invoke-MgLicenseUser

## SYNOPSIS
Reprocess all group-based license assignments for the user.
To learn more about group-based licensing, see What is group-based licensing in Microsoft Entra ID.
Also see Identify and resolve license assignment problems for a group in Microsoft Entra ID for more details.

> [!NOTE]
> To view the beta release of this cmdlet, view [Invoke-MgBetaLicenseUser](/powershell/module/Microsoft.Graph.Beta.Users.Actions/Invoke-MgBetaLicenseUser?view=graph-powershell-beta)

## SYNTAX

### License (Default)
```
Invoke-MgLicenseUser -UserId <String> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### LicenseViaIdentity
```
Invoke-MgLicenseUser -InputObject <IUsersActionsIdentity> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Reprocess all group-based license assignments for the user.
To learn more about group-based licensing, see What is group-based licensing in Microsoft Entra ID.
Also see Identify and resolve license assignment problems for a group in Microsoft Entra ID for more details.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | User.ReadWrite.All, Directory.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | User.ReadWrite.All, Directory.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Users.Actions

Invoke-MgLicenseUser -UserId $userId

```
This example shows how to use the Invoke-MgLicenseUser Cmdlet.


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
Parameter Sets: LicenseViaIdentity
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
Parameter Sets: License
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUser
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IUsersActionsIdentity>`: Identity Parameter
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/invoke-mglicenseuser](https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/invoke-mglicenseuser)

[https://learn.microsoft.com/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0)























