---
external help file: Microsoft.Graph.Devices.ServiceAnnouncement-help.xml
Module Name: Microsoft.Graph.Devices.ServiceAnnouncement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devices.serviceannouncement/invoke-mgunfavoriteserviceannouncementmessage
schema: 2.0.0
ms.subservice: service-communications
---

# Invoke-MgUnfavoriteServiceAnnouncementMessage

## SYNOPSIS
Remove the favorite status of serviceUpdateMessages for the signed in user.

> [!NOTE]
> To view the beta release of this cmdlet, view [Invoke-MgBetaUnfavoriteServiceAnnouncementMessage](/powershell/module/Microsoft.Graph.Beta.Devices.ServiceAnnouncement/Invoke-MgBetaUnfavoriteServiceAnnouncementMessage?view=graph-powershell-beta)

## SYNTAX

### UnfavoriteExpanded (Default)
```
Invoke-MgUnfavoriteServiceAnnouncementMessage [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-MessageIds <String[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Unfavorite
```
Invoke-MgUnfavoriteServiceAnnouncementMessage
 -Body <IPaths1U36FhAdminServiceannouncementMessagesMicrosoftGraphUnfavoritePostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Remove the favorite status of serviceUpdateMessages for the signed in user.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

$params = @{
	messageIds = @(
	"MC172851"
"MC167983"
)
}

Invoke-MgUnfavoriteServiceAnnouncementMessage -BodyParameter $params

```
This example shows how to use the Invoke-MgUnfavoriteServiceAnnouncementMessage Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UnfavoriteExpanded
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
Type: IPaths1U36FhAdminServiceannouncementMessagesMicrosoftGraphUnfavoritePostRequestbodyContentApplicationJsonSchema
Parameter Sets: Unfavorite
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

### -MessageIds


```yaml
Type: String[]
Parameter Sets: UnfavoriteExpanded
Aliases:

Required: False
Position: Named
Default value: None
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

### Microsoft.Graph.PowerShell.Models.IPaths1U36FhAdminServiceannouncementMessagesMicrosoftGraphUnfavoritePostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODY `<IPaths1U36FhAdminServiceannouncementMessagesMicrosoftGraphUnfavoritePostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[MessageIds <String- `[]`>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.devices.serviceannouncement/invoke-mgunfavoriteserviceannouncementmessage](https://learn.microsoft.com/powershell/module/microsoft.graph.devices.serviceannouncement/invoke-mgunfavoriteserviceannouncementmessage)

[https://learn.microsoft.com/graph/api/serviceupdatemessage-unfavorite?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/serviceupdatemessage-unfavorite?view=graph-rest-1.0)























