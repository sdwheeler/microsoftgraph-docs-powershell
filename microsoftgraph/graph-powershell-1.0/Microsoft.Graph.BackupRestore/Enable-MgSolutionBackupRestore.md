---
external help file: Microsoft.Graph.BackupRestore-help.xml
Module Name: Microsoft.Graph.BackupRestore
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.backuprestore/enable-mgsolutionbackuprestore
schema: 2.0.0
ms.subservice: m365-backup-storage
---

# Enable-MgSolutionBackupRestore

## SYNOPSIS
Enable the Microsoft 365 Backup Storage service for a tenant.

> [!NOTE]
> To view the beta release of this cmdlet, view [Enable-MgBetaSolutionBackupRestore](/powershell/module/Microsoft.Graph.Beta.BackupRestore/Enable-MgBetaSolutionBackupRestore?view=graph-powershell-beta)

## SYNTAX

### EnableExpanded (Default)
```
Enable-MgSolutionBackupRestore [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AppOwnerTenantId <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Enable
```
Enable-MgSolutionBackupRestore
 -BodyParameter <IPathsI0X7PjSolutionsBackuprestoreMicrosoftGraphEnablePostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Enable the Microsoft 365 Backup Storage service for a tenant.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: EnableExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppOwnerTenantId


```yaml
Type: String
Parameter Sets: EnableExpanded
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
Type: IPathsI0X7PjSolutionsBackuprestoreMicrosoftGraphEnablePostRequestbodyContentApplicationJsonSchema
Parameter Sets: Enable
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

### Microsoft.Graph.PowerShell.Models.IPathsI0X7PjSolutionsBackuprestoreMicrosoftGraphEnablePostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphServiceStatus
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsI0X7PjSolutionsBackuprestoreMicrosoftGraphEnablePostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AppOwnerTenantId <String>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.backuprestore/enable-mgsolutionbackuprestore](https://learn.microsoft.com/powershell/module/microsoft.graph.backuprestore/enable-mgsolutionbackuprestore)

[https://learn.microsoft.com/graph/api/backuprestoreroot-enable?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/backuprestoreroot-enable?view=graph-rest-1.0)
























