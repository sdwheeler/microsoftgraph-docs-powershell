---
external help file: Microsoft.Graph.Beta.DeviceManagement.Enrollment-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement.Enrollment
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/search-mgbetadevicemanagementimporteddeviceidentityexistingidentity
schema: 2.0.0
---

# Search-MgBetaDeviceManagementImportedDeviceIdentityExistingIdentity

## SYNOPSIS
Invoke action searchExistingIdentities

## SYNTAX

### SearchExpanded (Default)
```
Search-MgBetaDeviceManagementImportedDeviceIdentityExistingIdentity [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ImportedDeviceIdentities <IMicrosoftGraphImportedDeviceIdentity[]>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Search
```
Search-MgBetaDeviceManagementImportedDeviceIdentityExistingIdentity
 -BodyParameter <IPathsHi19O6DevicemanagementImporteddeviceidentitiesMicrosoftGraphSearchexistingidentitiesPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action searchExistingIdentities

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: SearchExpanded
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
Type: IPathsHi19O6DevicemanagementImporteddeviceidentitiesMicrosoftGraphSearchexistingidentitiesPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Search
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

### -ImportedDeviceIdentities

To construct, see NOTES section for IMPORTEDDEVICEIDENTITIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphImportedDeviceIdentity[]
Parameter Sets: SearchExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IPathsHi19O6DevicemanagementImporteddeviceidentitiesMicrosoftGraphSearchexistingidentitiesPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphImportedDeviceIdentity
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsHi19O6DevicemanagementImporteddeviceidentitiesMicrosoftGraphSearchexistingidentitiesPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ImportedDeviceIdentities <IMicrosoftGraphImportedDeviceIdentity- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedDateTime <DateTime?>]`: Created Date Time of the device
    - `[Description <String>]`: The description of the device
    - `[EnrollmentState <EnrollmentState?>]`: enrollmentState
    - `[ImportedDeviceIdentifier <String>]`: Imported Device Identifier
    - `[ImportedDeviceIdentityType <ImportedDeviceIdentityType?>]`: importedDeviceIdentityType
    - `[LastContactedDateTime <DateTime?>]`: Last Contacted Date Time of the device
    - `[LastModifiedDateTime <DateTime?>]`: Last Modified DateTime of the description
    - `[Platform <Platform?>]`: Supported platform types for policies.

IMPORTEDDEVICEIDENTITIES `<IMicrosoftGraphImportedDeviceIdentity- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CreatedDateTime <DateTime?>]`: Created Date Time of the device
  - `[Description <String>]`: The description of the device
  - `[EnrollmentState <EnrollmentState?>]`: enrollmentState
  - `[ImportedDeviceIdentifier <String>]`: Imported Device Identifier
  - `[ImportedDeviceIdentityType <ImportedDeviceIdentityType?>]`: importedDeviceIdentityType
  - `[LastContactedDateTime <DateTime?>]`: Last Contacted Date Time of the device
  - `[LastModifiedDateTime <DateTime?>]`: Last Modified DateTime of the description
  - `[Platform <Platform?>]`: Supported platform types for policies.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/search-mgbetadevicemanagementimporteddeviceidentityexistingidentity](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/search-mgbetadevicemanagementimporteddeviceidentityexistingidentity)
























