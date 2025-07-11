---
external help file: Microsoft.Graph.Groups-help.xml
Module Name: Microsoft.Graph.Groups
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.groups/new-mggroupownerbyref
schema: 2.0.0
ms.subservice: entra-groups
---

# New-MgGroupOwnerByRef

## SYNOPSIS
Add a user or service principal to a Microsoft 365 or security group's owners.
The owners are a set of users or service principals who are allowed to modify the group object.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaGroupOwnerByRef](/powershell/module/Microsoft.Graph.Beta.Groups/New-MgBetaGroupOwnerByRef?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgGroupOwnerByRef -GroupId <String> [-ResponseHeadersVariable <String>] -OdataId <String>
 [-AdditionalProperties <Hashtable>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgGroupOwnerByRef -GroupId <String> -BodyParameter <IReferenceCreate> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgGroupOwnerByRef -InputObject <IGroupsIdentity> [-ResponseHeadersVariable <String>] -OdataId <String>
 [-AdditionalProperties <Hashtable>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgGroupOwnerByRef -InputObject <IGroupsIdentity> -BodyParameter <IReferenceCreate>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Add a user or service principal to a Microsoft 365 or security group's owners.
The owners are a set of users or service principals who are allowed to modify the group object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Group.ReadWrite.All, Directory.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Group.ReadWrite.All, Directory.ReadWrite.All,  |

## EXAMPLES
### Example 1: Add an owner to a group

```powershell
$newGroupOwner =@{
  "@odata.id"= "https://graph.microsoft.com/v1.0/users/{4de19c17-6a28-4a91-86d1-f717c3c8c229}"
  }

New-MgGroupOwnerByRef -GroupId '1cb7317c-9c49-4dc8-a358-67ad8e95217c' -BodyParameter $newGroupOwner
```

In this example, the first command defines the value of the $newGroupOwner variable. The second command creates the value is an owner of the specified group.

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Type: IReferenceCreate
Parameter Sets: Create, CreateViaIdentity
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

### -GroupId
The unique identifier of group

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
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
Type: IGroupsIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OdataId
The entity reference URL of the resource.
For example, https://graph.microsoft.com/v1.0/directoryObjects/{id}.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: True
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

### Microsoft.Graph.PowerShell.Models.IGroupsIdentity
### Microsoft.Graph.PowerShell.Models.IReferenceCreate
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IReferenceCreate>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  OdataId `<String>`: The entity reference URL of the resource.
For example, https://graph.microsoft.com/v1.0/directoryObjects/{id}.

INPUTOBJECT `<IGroupsIdentity>`: Identity Parameter
  - `[AttachmentId <String>]`: The unique identifier of attachment
  - `[ConversationId <String>]`: The unique identifier of conversation
  - `[ConversationThreadId <String>]`: The unique identifier of conversationThread
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EndDateTime <String>]`: Usage: endDateTime='{endDateTime}'
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[GroupId <String>]`: The unique identifier of group
  - `[GroupLifecyclePolicyId <String>]`: The unique identifier of groupLifecyclePolicy
  - `[GroupSettingId <String>]`: The unique identifier of groupSetting
  - `[GroupSettingTemplateId <String>]`: The unique identifier of groupSettingTemplate
  - `[Interval <String>]`: Usage: interval='{interval}'
  - `[ListId <String>]`: Usage: listId='{listId}'
  - `[Path <String>]`: Usage: path='{path}'
  - `[PostId <String>]`: The unique identifier of post
  - `[ProfilePhotoId <String>]`: The unique identifier of profilePhoto
  - `[ResourceSpecificPermissionGrantId <String>]`: The unique identifier of resourceSpecificPermissionGrant
  - `[SiteId <String>]`: The unique identifier of site
  - `[StartDateTime <String>]`: Usage: startDateTime='{startDateTime}'
  - `[UniqueName <String>]`: Alternate key of group

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.groups/new-mggroupownerbyref](https://learn.microsoft.com/powershell/module/microsoft.graph.groups/new-mggroupownerbyref)

[https://learn.microsoft.com/graph/api/group-post-owners?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/group-post-owners?view=graph-rest-1.0)























