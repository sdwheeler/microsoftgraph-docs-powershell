---
external help file: Microsoft.Graph.Search-help.xml
Module Name: Microsoft.Graph.Search
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.search/remove-mgexternalconnection
schema: 2.0.0
ms.subservice: search
---

# Remove-MgExternalConnection

## SYNOPSIS
Deletes an externalConnection object.

> [!NOTE]
> To view the beta release of this cmdlet, view [Remove-MgBetaExternalConnection](/powershell/module/Microsoft.Graph.Beta.Search/Remove-MgBetaExternalConnection?view=graph-powershell-beta)

## SYNTAX

### Delete (Default)
```
Remove-MgExternalConnection -ExternalConnectionId <String> [-IfMatch <String>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### DeleteViaIdentity
```
Remove-MgExternalConnection -InputObject <ISearchIdentity> [-IfMatch <String>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Deletes an externalConnection object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | ExternalConnection.ReadWrite.OwnedBy, ExternalConnection.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | ExternalConnection.ReadWrite.OwnedBy, ExternalConnection.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Search

Remove-MgExternalConnection -ExternalConnectionId $externalConnectionId

```
This example shows how to use the Remove-MgExternalConnection Cmdlet.


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

### -ExternalConnectionId
The unique identifier of externalConnection

```yaml
Type: String
Parameter Sets: Delete
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

### -IfMatch
ETag

```yaml
Type: String
Parameter Sets: (All)
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
Type: ISearchIdentity
Parameter Sets: DeleteViaIdentity
Aliases:

Required: True
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

### Microsoft.Graph.PowerShell.Models.ISearchIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<ISearchIdentity>`: Identity Parameter
  - `[AcronymId <String>]`: The unique identifier of acronym
  - `[BookmarkId <String>]`: The unique identifier of bookmark
  - `[ConnectionOperationId <String>]`: The unique identifier of connectionOperation
  - `[ExternalActivityId <String>]`: The unique identifier of externalActivity
  - `[ExternalConnectionId <String>]`: The unique identifier of externalConnection
  - `[ExternalGroupId <String>]`: The unique identifier of externalGroup
  - `[ExternalItemId <String>]`: The unique identifier of externalItem
  - `[IdentityId <String>]`: The unique identifier of identity
  - `[QnaId <String>]`: The unique identifier of qna

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.search/remove-mgexternalconnection](https://learn.microsoft.com/powershell/module/microsoft.graph.search/remove-mgexternalconnection)

[https://learn.microsoft.com/graph/api/externalconnectors-externalconnection-delete?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/externalconnectors-externalconnection-delete?view=graph-rest-1.0)























