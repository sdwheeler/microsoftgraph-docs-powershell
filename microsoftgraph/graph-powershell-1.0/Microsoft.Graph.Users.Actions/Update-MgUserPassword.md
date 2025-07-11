---
external help file: Microsoft.Graph.Users.Actions-help.xml
Module Name: Microsoft.Graph.Users.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/update-mguserpassword
schema: 2.0.0
ms.subservice: entra-users
---

# Update-MgUserPassword

## SYNOPSIS
Update the signed-in user's password.
Any user can update their password without belonging to any administrator role.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaUserPassword](/powershell/module/Microsoft.Graph.Beta.Users.Actions/Update-MgBetaUserPassword?view=graph-powershell-beta)

## SYNTAX

### ChangeExpanded (Default)
```
Update-MgUserPassword -UserId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-CurrentPassword <String>] [-NewPassword <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Change
```
Update-MgUserPassword -UserId <String>
 -BodyParameter <IComponents89FyhbRequestbodiesChangepasswordrequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ChangeViaIdentityExpanded
```
Update-MgUserPassword -InputObject <IUsersActionsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CurrentPassword <String>] [-NewPassword <String>]
 [-Headers <IDictionary>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### ChangeViaIdentity
```
Update-MgUserPassword -InputObject <IUsersActionsIdentity>
 -BodyParameter <IComponents89FyhbRequestbodiesChangepasswordrequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the signed-in user's password.
Any user can update their password without belonging to any administrator role.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
	currentPassword = "xWwvJ]6NMw+bWH-d"
	newPassword = "0eM85N54wFxWwvJ]"
}

# A UPN can also be used as -UserId.
Update-MgUserPassword -UserId $userId -BodyParameter $params

```
This example shows how to use the Update-MgUserPassword Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: ChangeExpanded, ChangeViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter

To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IComponents89FyhbRequestbodiesChangepasswordrequestbodyContentApplicationJsonSchema
Parameter Sets: Change, ChangeViaIdentity
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

### -CurrentPassword


```yaml
Type: String
Parameter Sets: ChangeExpanded, ChangeViaIdentityExpanded
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IUsersActionsIdentity
Parameter Sets: ChangeViaIdentityExpanded, ChangeViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NewPassword


```yaml
Type: String
Parameter Sets: ChangeExpanded, ChangeViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

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
Parameter Sets: ChangeExpanded, Change
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

### Microsoft.Graph.PowerShell.Models.IComponents89FyhbRequestbodiesChangepasswordrequestbodyContentApplicationJsonSchema
### Microsoft.Graph.PowerShell.Models.IUsersActionsIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IComponents89FyhbRequestbodiesChangepasswordrequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CurrentPassword <String>]`:
  - `[NewPassword <String>]`:

INPUTOBJECT `<IUsersActionsIdentity>`: Identity Parameter
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/update-mguserpassword](https://learn.microsoft.com/powershell/module/microsoft.graph.users.actions/update-mguserpassword)

[https://learn.microsoft.com/graph/api/user-changepassword?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/user-changepassword?view=graph-rest-1.0)























