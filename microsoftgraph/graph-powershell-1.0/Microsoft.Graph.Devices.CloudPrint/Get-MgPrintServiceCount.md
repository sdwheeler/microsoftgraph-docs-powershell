---
external help file: Microsoft.Graph.Devices.CloudPrint-help.xml
Module Name: Microsoft.Graph.Devices.CloudPrint
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devices.cloudprint/get-mgprintservicecount
schema: 2.0.0
---

# Get-MgPrintServiceCount

## SYNOPSIS
Get the number of the resource

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaPrintServiceCount](/powershell/module/Microsoft.Graph.Beta.Devices.CloudPrint/Get-MgBetaPrintServiceCount?view=graph-powershell-beta)

## SYNTAX

```
Get-MgPrintServiceCount [-Filter <String>] [-Search <String>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

## DESCRIPTION
Get the number of the resource

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | PrintJob.ReadBasic, PrintSettings.ReadWrite.All, PrintSettings.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite.All, PrintJob.ReadWrite, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.Read, PrintJob.Create, PrinterShare.ReadWrite.All, PrinterShare.ReadBasic.All, PrinterShare.Read.All, Printer.ReadWrite.All, Printer.Read.All, Printer.Create, PrintConnector.ReadWrite.All, PrintConnector.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Not supported |

## EXAMPLES

## PARAMETERS

### -Filter
Filter items by property values

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

### -Search
Search items by search phrases

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Collections.IDictionary
## OUTPUTS

### System.Int32
## NOTES

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.devices.cloudprint/get-mgprintservicecount](https://learn.microsoft.com/powershell/module/microsoft.graph.devices.cloudprint/get-mgprintservicecount)
























