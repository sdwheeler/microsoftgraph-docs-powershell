---
external help file: Microsoft.Graph.Beta.Users.Actions-help.xml
Module Name: Microsoft.Graph.Beta.Users.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/confirm-mgbetausermembergroup
schema: 2.0.0
ms.subservice: entra-directory-management
---

# Confirm-MgBetaUserMemberGroup

## SYNOPSIS
Check for membership in a specified list of group IDs, and return from that list the IDs of groups where a specified object is a member.
The specified object can be of one of the following types:- user- group- service principal- organizational contact- device- directory object This function is transitive.
You can check up to a maximum of 20 groups per request.
This function supports all groups provisioned in Microsoft Entra ID.
Because Microsoft 365 groups cannot contain other groups, membership in a Microsoft 365 group is always direct.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Confirm-MgUserMemberGroup](/powershell/module/Microsoft.Graph.Users.Actions/Confirm-MgUserMemberGroup?view=graph-powershell-1.0)

## SYNTAX

### CheckExpanded (Default)
```
Confirm-MgBetaUserMemberGroup -UserId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-GroupIds <String[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Check
```
Confirm-MgBetaUserMemberGroup -UserId <String>
 -BodyParameter <IPathsDyyrb2UsersUserIdMicrosoftGraphCheckmembergroupsPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CheckViaIdentityExpanded
```
Confirm-MgBetaUserMemberGroup -InputObject <IUsersActionsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-GroupIds <String[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CheckViaIdentity
```
Confirm-MgBetaUserMemberGroup -InputObject <IUsersActionsIdentity>
 -BodyParameter <IPathsDyyrb2UsersUserIdMicrosoftGraphCheckmembergroupsPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Check for membership in a specified list of group IDs, and return from that list the IDs of groups where a specified object is a member.
The specified object can be of one of the following types:- user- group- service principal- organizational contact- device- directory object This function is transitive.
You can check up to a maximum of 20 groups per request.
This function supports all groups provisioned in Microsoft Entra ID.
Because Microsoft 365 groups cannot contain other groups, membership in a Microsoft 365 group is always direct.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Application.Read.All, User.ReadWrite.All, GroupMember.Read.All, User.Read.All, Application.ReadWrite.All, Device.Read.All, Directory.Read.All, Directory.ReadWrite.All, Group.Read.All, Group.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Application.Read.All, Application.ReadWrite.All, User.Read.All, GroupMember.Read.All, Group.ReadWrite.All, Group.Read.All, User.ReadWrite.All, Directory.Read.All, Device.ReadWrite.All, Device.Read.All, Directory.ReadWrite.All,  |

## EXAMPLES
### Example 1: Check group memberships for the signed-in user

```powershell

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	groupIds = @(
	"fee2c45b-915a-4a64-b130-f4eb9e75525e"
"4fe90ae7-065a-478b-9400-e0a0e1cbd540"
)
}

# A UPN can also be used as -UserId.
Confirm-MgBetaUserMemberGroup -UserId $userId -BodyParameter $params

```
This example will check group memberships for the signed-in user


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CheckExpanded, CheckViaIdentityExpanded
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
Type: IPathsDyyrb2UsersUserIdMicrosoftGraphCheckmembergroupsPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Check, CheckViaIdentity
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

### -GroupIds


```yaml
Type: String[]
Parameter Sets: CheckExpanded, CheckViaIdentityExpanded
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
Parameter Sets: CheckViaIdentityExpanded, CheckViaIdentity
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
Parameter Sets: CheckExpanded, Check
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

### Microsoft.Graph.Beta.PowerShell.Models.IPathsDyyrb2UsersUserIdMicrosoftGraphCheckmembergroupsPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.Beta.PowerShell.Models.IUsersActionsIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.String
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsDyyrb2UsersUserIdMicrosoftGraphCheckmembergroupsPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[GroupIds <String- `[]`>]`: 

INPUTOBJECT `<IUsersActionsIdentity>`: Identity Parameter
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/confirm-mgbetausermembergroup](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/confirm-mgbetausermembergroup)

[https://learn.microsoft.com/graph/api/directoryobject-checkmembergroups?view=graph-rest-beta](https://learn.microsoft.com/graph/api/directoryobject-checkmembergroups?view=graph-rest-beta)























