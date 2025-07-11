---
external help file: Microsoft.Graph.Beta.WindowsUpdates-help.xml
Module Name: Microsoft.Graph.Beta.WindowsUpdates
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.windowsupdates/invoke-mgbetaenrollwindowsupdatesupdatableasset
schema: 2.0.0
---

# Invoke-MgBetaEnrollWindowsUpdatesUpdatableAsset

## SYNOPSIS
Enroll updatableAsset resources in update management by Windows Autopatch.
You can enroll an azureADDevice resource in update management, but may not enroll an updatableAssetGroup in update management.
Enrolling a Microsoft Entra device in update management automatically creates an azureADDevice object if it does not already exist.
You can also use the method enrollAssetsById to enroll assets.

## SYNTAX

### EnrollExpanded (Default)
```
Invoke-MgBetaEnrollWindowsUpdatesUpdatableAsset [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Assets <IMicrosoftGraphWindowsUpdatesUpdatableAsset[]>]
 [-UpdateCategory <String>] [-Headers <IDictionary>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Enroll
```
Invoke-MgBetaEnrollWindowsUpdatesUpdatableAsset
 -Body <IPaths1T34IjjAdminWindowsUpdatesUpdatableassetsMicrosoftGraphWindowsupdatesEnrollassetsPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Enroll updatableAsset resources in update management by Windows Autopatch.
You can enroll an azureADDevice resource in update management, but may not enroll an updatableAssetGroup in update management.
Enrolling a Microsoft Entra device in update management automatically creates an azureADDevice object if it does not already exist.
You can also use the method enrollAssetsById to enroll assets.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | WindowsUpdates.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | WindowsUpdates.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: EnrollExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Assets

To construct, see NOTES section for ASSETS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsUpdatesUpdatableAsset[]
Parameter Sets: EnrollExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Body

To construct, see NOTES section for BODY properties and create a hash table.

```yaml
Type: IPaths1T34IjjAdminWindowsUpdatesUpdatableassetsMicrosoftGraphWindowsupdatesEnrollassetsPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Enroll
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

### -UpdateCategory
updateCategory

```yaml
Type: String
Parameter Sets: EnrollExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IPaths1T34IjjAdminWindowsUpdatesUpdatableassetsMicrosoftGraphWindowsupdatesEnrollassetsPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ASSETS `<IMicrosoftGraphWindowsUpdatesUpdatableAsset- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

BODY `<IPaths1T34IjjAdminWindowsUpdatesUpdatableassetsMicrosoftGraphWindowsupdatesEnrollassetsPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Assets <IMicrosoftGraphWindowsUpdatesUpdatableAsset- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[UpdateCategory <String>]`: updateCategory

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.windowsupdates/invoke-mgbetaenrollwindowsupdatesupdatableasset](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.windowsupdates/invoke-mgbetaenrollwindowsupdatesupdatableasset)
























