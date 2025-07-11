---
external help file: Microsoft.Graph.DirectoryObjects-help.xml
Module Name: Microsoft.Graph.DirectoryObjects
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.directoryobjects/get-mgdirectoryobjectavailableextensionproperty
schema: 2.0.0
ms.subservice: entra-directory-management
---

# Get-MgDirectoryObjectAvailableExtensionProperty

## SYNOPSIS
Return all directory extension definitions that have been registered in a directory, including through multi-tenant apps.
The following entities support extension properties:

## SYNTAX

### GetExpanded (Default)
```
Get-MgDirectoryObjectAvailableExtensionProperty [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-IsSyncedFromOnPremises] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Get
```
Get-MgDirectoryObjectAvailableExtensionProperty
 -BodyParameter <IPaths1Izu2OlDirectoryobjectsMicrosoftGraphGetavailableextensionpropertiesPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Return all directory extension definitions that have been registered in a directory, including through multi-tenant apps.
The following entities support extension properties:

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Directory.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Directory.Read.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
}

Get-MgDirectoryObjectAvailableExtensionProperty -BodyParameter $params

```
This example shows how to use the Get-MgDirectoryObjectAvailableExtensionProperty Cmdlet.


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
Type: IPaths1Izu2OlDirectoryobjectsMicrosoftGraphGetavailableextensionpropertiesPostRequestbodyContentApplicationJsonSchema
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

### -IsSyncedFromOnPremises


```yaml
Type: SwitchParameter
Parameter Sets: GetExpanded
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

### Microsoft.Graph.PowerShell.Models.IPaths1Izu2OlDirectoryobjectsMicrosoftGraphGetavailableextensionpropertiesPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphExtensionProperty
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths1Izu2OlDirectoryobjectsMicrosoftGraphGetavailableextensionpropertiesPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsSyncedFromOnPremises <Boolean?>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.directoryobjects/get-mgdirectoryobjectavailableextensionproperty](https://learn.microsoft.com/powershell/module/microsoft.graph.directoryobjects/get-mgdirectoryobjectavailableextensionproperty)

[https://learn.microsoft.com/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-1.0)























