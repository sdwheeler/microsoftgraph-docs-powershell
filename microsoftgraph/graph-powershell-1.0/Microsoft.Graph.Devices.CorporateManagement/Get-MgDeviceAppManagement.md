---
external help file: Microsoft.Graph.Devices.CorporateManagement-help.xml
Module Name: Microsoft.Graph.Devices.CorporateManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/get-mgdeviceappmanagement
schema: 2.0.0
ms.subservice: intune
---

# Get-MgDeviceAppManagement

## SYNOPSIS
Read properties and relationships of the deviceAppManagement object.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaDeviceAppManagement](/powershell/module/Microsoft.Graph.Beta.Devices.CorporateManagement/Get-MgBetaDeviceAppManagement?view=graph-powershell-beta)

## SYNTAX

```
Get-MgDeviceAppManagement [-ExpandProperty <String[]>] [-Property <String[]>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Read properties and relationships of the deviceAppManagement object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementApps.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementApps.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Devices.CorporateManagement

Get-MgDeviceAppManagement

```
This example shows how to use the Get-MgDeviceAppManagement Cmdlet.


## PARAMETERS

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Expand

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

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphDeviceAppManagement
## NOTES

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/get-mgdeviceappmanagement](https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/get-mgdeviceappmanagement)

[https://learn.microsoft.com/graph/api/intune-unlock-deviceappmanagement-get?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/intune-unlock-deviceappmanagement-get?view=graph-rest-1.0)























