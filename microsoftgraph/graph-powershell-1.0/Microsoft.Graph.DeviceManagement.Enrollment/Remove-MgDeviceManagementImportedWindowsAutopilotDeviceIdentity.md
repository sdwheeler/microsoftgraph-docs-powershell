---
external help file: Microsoft.Graph.DeviceManagement.Enrollment-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Enrollment
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.enrollment/remove-mgdevicemanagementimportedwindowsautopilotdeviceidentity
schema: 2.0.0
ms.subservice: intune
---

# Remove-MgDeviceManagementImportedWindowsAutopilotDeviceIdentity

## SYNOPSIS
Deletes a importedWindowsAutopilotDeviceIdentity.

> [!NOTE]
> To view the beta release of this cmdlet, view [Remove-MgBetaDeviceManagementImportedWindowsAutopilotDeviceIdentity](/powershell/module/Microsoft.Graph.Beta.DeviceManagement.Enrollment/Remove-MgBetaDeviceManagementImportedWindowsAutopilotDeviceIdentity?view=graph-powershell-beta)

## SYNTAX

### Delete (Default)
```
Remove-MgDeviceManagementImportedWindowsAutopilotDeviceIdentity
 -ImportedWindowsAutopilotDeviceIdentityId <String> [-IfMatch <String>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### DeleteViaIdentity
```
Remove-MgDeviceManagementImportedWindowsAutopilotDeviceIdentity
 -InputObject <IDeviceManagementEnrollmentIdentity> [-IfMatch <String>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Deletes a importedWindowsAutopilotDeviceIdentity.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementServiceConfig.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementServiceConfig.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrollment

Remove-MgDeviceManagementImportedWindowsAutopilotDeviceIdentity -ImportedWindowsAutopilotDeviceIdentityId $importedWindowsAutopilotDeviceIdentityId

```
This example shows how to use the Remove-MgDeviceManagementImportedWindowsAutopilotDeviceIdentity Cmdlet.


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

### -ImportedWindowsAutopilotDeviceIdentityId
The unique identifier of importedWindowsAutopilotDeviceIdentity

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IDeviceManagementEnrollmentIdentity
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

### Microsoft.Graph.PowerShell.Models.IDeviceManagementEnrollmentIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IDeviceManagementEnrollmentIdentity>`: Identity Parameter
  - `[DeviceEnrollmentConfigurationId <String>]`: The unique identifier of deviceEnrollmentConfiguration
  - `[EnrollmentConfigurationAssignmentId <String>]`: The unique identifier of enrollmentConfigurationAssignment
  - `[ImportedWindowsAutopilotDeviceIdentityId <String>]`: The unique identifier of importedWindowsAutopilotDeviceIdentity
  - `[WindowsAutopilotDeviceIdentityId <String>]`: The unique identifier of windowsAutopilotDeviceIdentity

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.enrollment/remove-mgdevicemanagementimportedwindowsautopilotdeviceidentity](https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.enrollment/remove-mgdevicemanagementimportedwindowsautopilotdeviceidentity)

[https://learn.microsoft.com/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentity-delete?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentity-delete?view=graph-rest-1.0)























