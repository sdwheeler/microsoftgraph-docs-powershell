---
external help file: Microsoft.Graph.Beta.DirectoryObjects-help.xml
Module Name: Microsoft.Graph.Beta.DirectoryObjects
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.directoryobjects/confirm-mgbetadirectoryobjectmemberobject
schema: 2.0.0
---

# Confirm-MgBetaDirectoryObjectMemberObject

## SYNOPSIS
Invoke action checkMemberObjects

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Confirm-MgDirectoryObjectMemberObject](/powershell/module/Microsoft.Graph.DirectoryObjects/Confirm-MgDirectoryObjectMemberObject?view=graph-powershell-1.0)

## SYNTAX

### CheckExpanded (Default)
```
Confirm-MgBetaDirectoryObjectMemberObject -DirectoryObjectId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Ids <String[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Check
```
Confirm-MgBetaDirectoryObjectMemberObject -DirectoryObjectId <String>
 -BodyParameter <IPaths1B1K3OoDirectoryobjectsDirectoryobjectIdMicrosoftGraphCheckmemberobjectsPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CheckViaIdentityExpanded
```
Confirm-MgBetaDirectoryObjectMemberObject -InputObject <IDirectoryObjectsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Ids <String[]>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CheckViaIdentity
```
Confirm-MgBetaDirectoryObjectMemberObject -InputObject <IDirectoryObjectsIdentity>
 -BodyParameter <IPaths1B1K3OoDirectoryobjectsDirectoryobjectIdMicrosoftGraphCheckmemberobjectsPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action checkMemberObjects

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Application.Read.All, User.ReadWrite.All, User.Read, User.Read.All, Application.ReadWrite.All, Device.Read.All, Directory.Read.All, Directory.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, GroupMember.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Application.Read.All, Application.ReadWrite.All, User.Read.All, GroupMember.Read.All, Group.ReadWrite.All, Group.Read.All, User.ReadWrite.All, Directory.Read.All, Device.ReadWrite.All, Device.Read.All, Directory.ReadWrite.All,  |

## EXAMPLES

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
Type: IPaths1B1K3OoDirectoryobjectsDirectoryobjectIdMicrosoftGraphCheckmemberobjectsPostRequestbodyContentApplicationJsonSchema
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

### -DirectoryObjectId
The unique identifier of directoryObject

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

### -Ids


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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IDirectoryObjectsIdentity
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

### Microsoft.Graph.Beta.PowerShell.Models.IDirectoryObjectsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IPaths1B1K3OoDirectoryobjectsDirectoryobjectIdMicrosoftGraphCheckmemberobjectsPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.String
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths1B1K3OoDirectoryobjectsDirectoryobjectIdMicrosoftGraphCheckmemberobjectsPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Ids <String- `[]`>]`: 

INPUTOBJECT `<IDirectoryObjectsIdentity>`: Identity Parameter
  - `[CertificateAuthorityDetailId <String>]`: The unique identifier of certificateAuthorityDetail
  - `[CertificateBasedAuthPkiId <String>]`: The unique identifier of certificateBasedAuthPki
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.directoryobjects/confirm-mgbetadirectoryobjectmemberobject](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.directoryobjects/confirm-mgbetadirectoryobjectmemberobject)
























