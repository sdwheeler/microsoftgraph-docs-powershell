---
external help file: Microsoft.Graph.Beta.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Beta.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/get-mgbetadirectoryroleuserownedobject
schema: 2.0.0
ms.subservice: entra-directory-management
---

# Get-MgBetaDirectoryRoleUserOwnedObject

## SYNOPSIS
Retrieve a list of recently deleted application and group objects owned by the specified user.
This API returns up to 1,000 deleted objects owned by the user, sorted by ID, and doesn't support pagination.

## SYNTAX

### GetExpanded (Default)
```
Get-MgBetaDirectoryRoleUserOwnedObject [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Type <String>] [-UserId <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Get
```
Get-MgBetaDirectoryRoleUserOwnedObject
 -BodyParameter <IPathsRx7DjhDirectoryrolesMicrosoftGraphGetuserownedobjectsPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Retrieve a list of recently deleted application and group objects owned by the specified user.
This API returns up to 1,000 deleted objects owned by the user, sorted by ID, and doesn't support pagination.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: GetExpanded
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
Type: IPathsRx7DjhDirectoryrolesMicrosoftGraphGetuserownedobjectsPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Get
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

### -Type


```yaml
Type: String
Parameter Sets: GetExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId


```yaml
Type: String
Parameter Sets: GetExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IPathsRx7DjhDirectoryrolesMicrosoftGraphGetuserownedobjectsPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDirectoryObject
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsRx7DjhDirectoryrolesMicrosoftGraphGetuserownedobjectsPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Type <String>]`: 
  - `[UserId <String>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/get-mgbetadirectoryroleuserownedobject](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/get-mgbetadirectoryroleuserownedobject)

[https://learn.microsoft.com/graph/api/directory-deleteditems-getuserownedobjects?view=graph-rest-beta](https://learn.microsoft.com/graph/api/directory-deleteditems-getuserownedobjects?view=graph-rest-beta)
























